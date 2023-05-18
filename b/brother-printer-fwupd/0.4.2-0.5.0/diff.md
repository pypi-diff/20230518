# Comparing `tmp/brother_printer_fwupd-0.4.2.tar.gz` & `tmp/brother_printer_fwupd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brother_printer_fwupd-0.4.2.tar", max compression
+gzip compressed data, was "brother_printer_fwupd-0.5.0.tar", max compression
```

## Comparing `brother_printer_fwupd-0.4.2.tar` & `brother_printer_fwupd-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    35150 2019-05-05 22:45:01.929067 brother_printer_fwupd-0.4.2/LICENSE
--rw-r--r--   0        0        0       75 2022-06-04 19:12:12.377682 brother_printer_fwupd-0.4.2/brother_printer_fwupd/__init__.py
--rwxr-xr-x   0        0        0     4793 2022-06-04 20:29:54.810943 brother_printer_fwupd-0.4.2/brother_printer_fwupd/__main__.py
--rw-r--r--   0        0        0     6963 2022-06-04 20:12:02.331660 brother_printer_fwupd-0.4.2/brother_printer_fwupd/autodiscover_printer.py
--rw-r--r--   0        0        0     3815 2022-06-04 20:20:18.929338 brother_printer_fwupd-0.4.2/brother_printer_fwupd/firmware_downloader.py
--rw-r--r--   0        0        0      723 2020-12-31 17:15:31.520308 brother_printer_fwupd-0.4.2/brother_printer_fwupd/firmware_uploader.py
--rw-r--r--   0        0        0     1732 2022-06-04 20:20:18.909143 brother_printer_fwupd-0.4.2/brother_printer_fwupd/models.py
--rw-r--r--   0        0        0     3050 2022-06-04 20:30:23.818775 brother_printer_fwupd-0.4.2/brother_printer_fwupd/snmp_info.py
--rw-r--r--   0        0        0     3831 2022-06-04 19:27:33.860010 brother_printer_fwupd-0.4.2/brother_printer_fwupd/utils.py
--rw-r--r--   0        0        0      934 2022-06-04 20:36:31.717348 brother_printer_fwupd-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1139 2022-06-04 20:42:45.765420 brother_printer_fwupd-0.4.2/setup.py
--rw-r--r--   0        0        0     1014 2022-06-04 20:42:45.765675 brother_printer_fwupd-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35150 2019-05-05 22:45:01.929067 brother_printer_fwupd-0.5.0/LICENSE
+-rw-r--r--   0        0        0       75 2022-06-04 19:12:12.377682 brother_printer_fwupd-0.5.0/brother_printer_fwupd/__init__.py
+-rwxr-xr-x   0        0        0     6098 2023-05-18 13:36:05.427176 brother_printer_fwupd-0.5.0/brother_printer_fwupd/__main__.py
+-rw-r--r--   0        0        0     7080 2023-05-18 13:19:45.294187 brother_printer_fwupd-0.5.0/brother_printer_fwupd/autodiscover_printer.py
+-rw-r--r--   0        0        0     3128 2023-05-18 13:19:29.797478 brother_printer_fwupd-0.5.0/brother_printer_fwupd/firmware_downloader.py
+-rw-r--r--   0        0        0      739 2023-05-18 11:50:56.235324 brother_printer_fwupd-0.5.0/brother_printer_fwupd/firmware_uploader.py
+-rw-r--r--   0        0        0     1718 2023-05-18 11:55:02.716491 brother_printer_fwupd-0.5.0/brother_printer_fwupd/models.py
+-rw-r--r--   0        0        0     3050 2022-06-04 20:30:23.818775 brother_printer_fwupd-0.5.0/brother_printer_fwupd/snmp_info.py
+-rw-r--r--   0        0        0     5853 2023-05-18 13:37:45.074134 brother_printer_fwupd-0.5.0/brother_printer_fwupd/utils.py
+-rw-r--r--   0        0        0      875 2023-05-18 11:31:53.701264 brother_printer_fwupd-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 brother_printer_fwupd-0.5.0/PKG-INFO
```

### Comparing `brother_printer_fwupd-0.4.2/LICENSE` & `brother_printer_fwupd-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.4.2/brother_printer_fwupd/__main__.py` & `brother_printer_fwupd-0.5.0/brother_printer_fwupd/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,165 +1,224 @@
 #!/usr/bin/env python3
 """
 Script to update the firmware of some Brother printers (e. g. MFC).
 """
 
 import argparse
+import logging
 import sys
 import typing
-import logging
+import webbrowser
+from pathlib import Path
 
-PrinterDiscoverer: typing.Optional[typing.Type] = None
-try:
-    from .autodiscover_printer import PrinterDiscoverer
-except ImportError:
-    pass
+import termcolor
 
+from . import ISSUE_URL
+from .autodiscover_printer import PrinterDiscoverer
 from .firmware_downloader import download_fw, get_download_url
 from .firmware_uploader import upload_fw
-from .snmp_info import get_snmp_info
-from .utils import gooey_if_exists, LOGGER
 from .models import FWInfo, SNMPPrinterInfo
+from .snmp_info import get_snmp_info
+from .utils import (
+    CONSOLE_LOG_HANDLER,
+    LOGGER,
+    GitHubIssueReporter,
+    get_running_os,
+    gooey_if_exists,
+)
 
 if typing.TYPE_CHECKING:
     from .models import IPAddress
 
 
+RUNNING_OS = get_running_os()
+
+
 @gooey_if_exists
 def parse_args():
     """Parse command line args."""
     parser = argparse.ArgumentParser(
         prog=__file__,
         description=__doc__.strip().splitlines()[0],
     )
-    if PrinterDiscoverer is None:
-        discovery_available = False
-        blurb = "required, because zeroconf is not available"
-    else:
-        discovery_available = True
-        blurb = "default: autodiscover via mdns"
     parser.add_argument(
         "-p",
         "--printer",
-        required=not discovery_available,
+        dest="printer",
         metavar="host",
         default=None,
-        help=f"IP Address or hostname of the printer ({blurb}).",
-    )
-    parser.add_argument(
-        "--community",
-        "-c",
-        default="public",
-        help="SNMP Community string for the printer (default: '%(default)s').",
-    )
-    parser.add_argument(
-        "--fw-file",
-        "-f",
-        default="firmware.djf",
-        help="File name for the downloaded firmware (default: '%(default)s').",
-    )
-    parser.add_argument(
-        "--os",
-        type=str.upper,
-        choices=["WINDOWS", "MAC", "LINUX"],
-        help="Operating system to report when downloading firmware (default: autodetect)",
+        help="IP Address or hostname of the printer (default: autodiscover via mdns).",
     )
     parser.add_argument(
         "--model",
+        dest="model",
         type=str,
         help="Skip SNMP scanning by directly specifying the printer model.",
     )
     parser.add_argument(
         "--serial",
+        dest="serial",
         type=str,
         help="Skip SNMP scanning by directly specifying the printer serial.",
     )
     parser.add_argument(
         "--spec",
+        dest="spec",
         type=str,
         help="Skip SNMP scanning by directly specifying the printer spec.",
     )
     parser.add_argument(
         "--fw",
         "--fw-versions",
         dest="fw_versions",
         nargs="*",
         default=list[FWInfo](),
         type=FWInfo.from_str,
         help="Skip SNMP scanning by directly specifying the firmware parts to update.",
     )
     parser.add_argument(
+        "-c",
+        "--community",
+        dest="community",
+        default="public",
+        help="SNMP Community string for the printer (default: '%(default)s').",
+    )
+    parser.add_argument(
+        "-f",
+        "-o",
+        "--fw-file",
+        type=Path,
+        dest="fw_file",
+        default="firmware.djf",
+        help="File name for the downloaded firmware (default: '%(default)s').",
+    )
+    parser.add_argument(
+        "--os",
+        dest="os",
+        type=str.upper,
+        default=RUNNING_OS,
+        choices=["WINDOWS", "MAC", "LINUX"],
+        help="Operating system to report when downloading firmware (default: '%(default)s').",
+    )
+    parser.add_argument(
+        "--download-only",
+        dest="download_only",
+        action="store_true",
+        help="Do no install update but download firmware and save it unter the path given with --fw-file.",
+    )
+    parser.add_argument(
         "--debug",
+        dest="debug",
         action="store_true",
         help="Print debug messages",
     )
 
     return parser.parse_args()
 
 
 def main():
+    """Run the program."""
+
+    def handler_cb(report_url: str):
+        LOGGER.error("This might be a bug.")
+
+        while True:
+            ret = (
+                input(
+                    termcolor.colored(
+                        "Do you want open an issue? [yN] ", color="yellow"
+                    )
+                )
+                .strip()
+                .lower()
+            )
+
+            if ret.lower() == "y":
+                webbrowser.open(report_url)
+
+                return
+            elif ret.lower() == "n" or not ret:
+                return
+
+    with GitHubIssueReporter(
+        logger=LOGGER,
+        issue_url=ISSUE_URL,
+        handler_cb=handler_cb,
+    ):
+        run()
+
+
+def run():
     """Do a firmware upgrade."""
     args = parse_args()
 
-    LOGGER.setLevel(logging.DEBUG if args.debug else logging.INFO)
+    CONSOLE_LOG_HANDLER.setLevel(logging.DEBUG if args.debug else logging.INFO)
 
     printer_ip: typing.Optional["IPAddress"] = args.printer
-    upload_port: typing.Optional[int] = None
+    upload_port: int | None = None
+    use_snmp = (
+        not args.model or not args.serial or not args.spec or not args.fw_versions
+    )
+    printer_ip_required = use_snmp or not args.download_only
 
-    if not printer_ip:
+    if not printer_ip and printer_ip_required:
         LOGGER.info("Discovering printer via MDNS.")
         discoverer = PrinterDiscoverer()
         mdns_printer_info = discoverer.run_cli()
 
         if mdns_printer_info:
             printer_ip = mdns_printer_info.ip_addr
             upload_port = mdns_printer_info.port
 
-    if not printer_ip:
+    if not printer_ip and printer_ip_required:
         LOGGER.critical("No printer given or found.")
         sys.exit(1)
 
-    if args.model and args.serial and args.spec and args.fw_versions:
+    assert printer_ip
+
+    if use_snmp:
+        LOGGER.info("Querying printer info via SNMP.")
+        printer_info = get_snmp_info(target=printer_ip, community=args.community)
+    else:
         printer_info = SNMPPrinterInfo(
             model=args.model,
             serial=args.serial,
             spec=args.spec,
             fw_versions=args.fw_versions,
         )
-        snmp_used = False
-    else:
-        LOGGER.info("Querying printer info via SNMP.")
-        printer_info = get_snmp_info(target=printer_ip, community=args.community)
-        snmp_used = True
 
     versions_str = ", ".join(str(fw_info) for fw_info in printer_info.fw_versions)
     LOGGER.success(
         "%s %s with following firmware version(s): %s",
-        "Detected" if snmp_used else "Using",
+        "Detected" if use_snmp else "Using",
         printer_info.model,
         versions_str,
     )
     LOGGER.info("Querying firmware download URL from Brother update API.")
-    download_url: typing.Optional[str] = None
+    download_url: str | None = None
 
     for fw_part in printer_info.fw_versions:
         download_url = get_download_url(
             printer_info=printer_info,
             firmid=str(fw_part.firmid),
             reported_os=args.os,
         )
 
         if not download_url:
             continue
 
         LOGGER.debug("  Download URL is %s", download_url)
         LOGGER.success("Downloading firmware file.")
         download_fw(url=download_url, dst=args.fw_file)
-        LOGGER.info("Uploading firmware file to printer via jetdirect.")
-        upload_fw(target=printer_ip, port=upload_port, file_name=args.fw_file)
-        input("Continue? ")
+
+        if args.download_only:
+            LOGGER.info("Skipping firmware upload due to --download-only")
+        else:
+            LOGGER.info("Uploading firmware file to printer via jetdirect.")
+            upload_fw(target=printer_ip, port=upload_port, file_path=args.fw_file)
+            input("Continue? ")
 
     LOGGER.success("Done.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `brother_printer_fwupd-0.4.2/brother_printer_fwupd/autodiscover_printer.py` & `brother_printer_fwupd-0.5.0/brother_printer_fwupd/autodiscover_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,36 +3,33 @@
 # pylint: disable=C0103
 # pylint: disable=R1723
 
 import ipaddress
 import typing
 
 import termcolor
-
 import zeroconf
-from .models import MDNSPrinterInfo
-from .utils import clear_screen, LOGGER
 
-if typing.TYPE_CHECKING:
-    from .models import IPAddress
+from .models import MDNSPrinterInfo
+from .utils import LOGGER, clear_screen
 
 ZEROCONF_SERVICE_DOMAIN = "_pdl-datastream._tcp.local."
 
 termcolor.ATTRIBUTES["italic"] = 3  # type: ignore
 
 
 class PrinterDiscoverer(zeroconf.ServiceListener):
     """Discoverer of printers."""
 
     def __init__(self):
-        self._printers: typing.List[MDNSPrinterInfo] = []
+        self._printers: list[MDNSPrinterInfo] = list[MDNSPrinterInfo]()
         self._zc = zeroconf.Zeroconf()
         self._mode = "CLI"
         self._invalid_answer = False
-        self._browser: typing.Optional[zeroconf.ServiceBrowser] = None
+        self._browser: zeroconf.ServiceBrowser | None = None
 
     def remove_service(self, zc: zeroconf.Zeroconf, type_: str, name: str):
         LOGGER.debug(f"Service {name} removed")
         self._remove_printer_infos_by_name(name)
 
         if self._mode == "CLI":
             self._update_screen()
@@ -166,20 +163,26 @@
             termcolor.cprint(
                 f"Your choice {range_str}:",
                 attrs=["bold"],
                 end=" ",
                 flush=True,
             )
         else:
-            termcolor.cprint("No printers found yet. [Enter: Cancel]", attrs=["italic"])
+            termcolor.cprint(
+                "No printers found yet.", "yellow", attrs=["italic"], end=" "
+            )
+            termcolor.cprint(
+                "Run with --printer=<ip> to skip autodiscovery. [Enter: Cancel]",
+                attrs=["italic"],
+            )
 
-    def run_cli(self) -> typing.Optional[MDNSPrinterInfo]:
+    def run_cli(self) -> MDNSPrinterInfo | None:
         """Run as interactive terminal application."""
         self._mode = "CLI"
-        choice: typing.Optional[int] = None
+        choice: int | None = None
         self._run()
         self._update_screen()
 
         try:
             while True:
                 inpt = input().strip()
```

### Comparing `brother_printer_fwupd-0.4.2/brother_printer_fwupd/firmware_downloader.py` & `brother_printer_fwupd-0.5.0/brother_printer_fwupd/firmware_downloader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 """Logic to download the correct firmware from the official Brother server."""
-import sys
 import typing
-import logging
+from pathlib import Path
 
 import requests
 from bs4 import BeautifulSoup
 
-from . import ISSUE_URL
 from .utils import LOGGER
 
 if typing.TYPE_CHECKING:
     from .models import SNMPPrinterInfo
 
 FW_UPDATE_URL = (
     "https://firmverup.brother.co.jp/kne_bh7_update_nt_ssl/ifax2.asmx/fileUpdate"
 )
 
 
 def get_download_url(
     printer_info: "SNMPPrinterInfo",
+    reported_os: str,
     firmid: str = "MAIN",
-    reported_os: typing.Optional[str] = None,
-) -> typing.Optional[str]:
+) -> str | None:
     """Get the firmware download URL for the target printer."""
     firm_info = ""
 
     for fw_info in printer_info.fw_versions:
         firm_info += f"""
         <FIRM>
             <ID>{fw_info.firmid}</ID>
             <VERSION>{fw_info.firmver}</VERSION>
         </FIRM>
         """
 
-    if reported_os is None:
-        if sys.platform.startswith("win") or sys.platform.startswith("cygwin"):
-            reported_os = "WINDOWS"
-        elif sys.platform.startswith("darwin"):
-            reported_os = "MAC"
-        else:
-            reported_os = "LINUX"
-
     api_data = f"""
 <REQUESTINFO>
     <FIRMUPDATETOOLINFO>
         <FIRMCATEGORY>{firmid}</FIRMCATEGORY>
         <OS>{reported_os}</OS>
         <INSPECTMODE>1</INSPECTMODE>
     </FIRMUPDATETOOLINFO>
@@ -84,41 +74,33 @@
         versioncheck_val = versioncheck[0].text
         if versioncheck_val == "0":
             LOGGER.info("It seems that a firmware update is required for %s", firmid)
         elif versioncheck_val == "1":
             LOGGER.success("Firmware part %s seems to be up to date.", firmid)
             return None
         else:
-            LOGGER.error("Unknown versioncheck response for firmid=%s.", firmid)
-            LOGGER.error("There seems to be a bug.")
-            if LOGGER.level > logging.DEBUG:
-                LOGGER.error(
-                    "Run again with --debug and open an issue. Append the full output."
-                )
-            else:
-                LOGGER.error("Open an issue with the full debug output: %s", ISSUE_URL)
-            return None
+            raise ValueError(f"Unknown versioncheck response for firmid={firmid}.")
 
     path = resp_xml.find("PATH")
     if not path:
         LOGGER.warning("Did not receive download url for %s.", firmid)
         LOGGER.warning("Either this firmware part is up to date or there is a bug.")
         return None
 
     return path.text
 
 
-def download_fw(url: str, dst: str = "firmware.djf"):
+def download_fw(url: str, dst: Path = Path("firmware.djf")):
     """Download the firmware."""
     resp = requests.get(url, stream=True)
     resp.raise_for_status()
     total_size = int(resp.headers.get("content-length", 0))
     size_written = 0
     chunk_size = 8192
 
-    with open(dst, "wb") as out:
+    with dst.open("wb") as out:
         for chunk in resp.iter_content(chunk_size):
             size_written += out.write(chunk)
             progress = size_written / total_size * 100
             print(f"\r{progress: 5.1f} %", end="", flush=True)
 
     print()
```

### Comparing `brother_printer_fwupd-0.4.2/brother_printer_fwupd/firmware_uploader.py` & `brother_printer_fwupd-0.5.0/brother_printer_fwupd/firmware_uploader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Upload firmware to the brinter."""
 import socket
-import typing
+from pathlib import Path
 
 from .models import IPAddress
 
 PORT_SERVICE_NAME = "pdl-datastream"
 
 
 def upload_fw(
-    target: IPAddress, port: typing.Optional[int], file_name: str = "firmware.djf"
+    target: IPAddress,
+    port: int | None,
+    file_path: Path = Path("firmware.djf"),
 ):
     """
     Upload the firmware to the printer via PDL Datastream / JetDirect.
 
     Equals:
     ```
     cat LZ5413_P.djf | nc lp.local 9100
     ```
     """
     port = port if port else socket.getservbyname(PORT_SERVICE_NAME)
     addr_info = socket.getaddrinfo(str(target), port, 0, 0, socket.SOL_TCP)[0]
     with socket.socket(addr_info[0], addr_info[1], 0) as sock:
         sock.connect(addr_info[4])
 
-        with open(file_name, "rb") as fw_file:
+        with file_path.open("rb") as fw_file:
             sock.sendfile(fw_file)
```

### Comparing `brother_printer_fwupd-0.4.2/brother_printer_fwupd/snmp_info.py` & `brother_printer_fwupd-0.5.0/brother_printer_fwupd/snmp_info.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.4.2/pyproject.toml` & `brother_printer_fwupd-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "brother_printer_fwupd"
-version = "0.4.2"
+version = "0.5.0"
 description = "Script to update the firmware of some Brother printers (e. g. MFC)."
 authors = ["sedrubal <dev@sedrubal.de>"]
 repository = "https://github.com/sedrubal/brother_printer_fwupd.git"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pysnmp = "^4.4.12"
 requests = "^2.27.1"
 BeautifulSoup4 = "^4.9.1"
 Gooey = { version = "^1.0.3", optional = true }
 lxml = "^4.9.0"
-zeroconf = { version = "^0.28.7", optional = true }
+zeroconf = "^0.28.7"
 termcolor = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.14.0"
 mypy = "^0.960"
 pre-commit = "^2.19.0"
 black = "^22.3.0"
@@ -26,11 +26,10 @@
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.extras]
 graphical = ["Gooey"]
-autodiscover = ["zeroconf"]
 
 [tool.poetry.scripts]
 brother_printer_fwupd = 'brother_printer_fwupd.__main__:main'
```

### Comparing `brother_printer_fwupd-0.4.2/PKG-INFO` & `brother_printer_fwupd-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: brother-printer-fwupd
-Version: 0.4.2
+Version: 0.5.0
 Summary: Script to update the firmware of some Brother printers (e. g. MFC).
 Home-page: https://github.com/sedrubal/brother_printer_fwupd.git
 License: GPL-3.0-or-later
 Author: sedrubal
 Author-email: dev@sedrubal.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: autodiscover
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: graphical
 Requires-Dist: BeautifulSoup4 (>=4.9.1,<5.0.0)
-Requires-Dist: Gooey (>=1.0.3,<2.0.0); extra == "graphical"
+Requires-Dist: Gooey (>=1.0.3,<2.0.0) ; extra == "graphical"
 Requires-Dist: lxml (>=4.9.0,<5.0.0)
 Requires-Dist: pysnmp (>=4.4.12,<5.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
-Requires-Dist: zeroconf (>=0.28.7,<0.29.0); extra == "autodiscover"
+Requires-Dist: zeroconf (>=0.28.7,<0.29.0)
 Project-URL: Repository, https://github.com/sedrubal/brother_printer_fwupd.git
```


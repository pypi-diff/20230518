# Comparing `tmp/donjon-scaffold-0.7.7.tar.gz` & `tmp/donjon-scaffold-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/donjon-scaffold-0.7.7.tar", last modified: Thu Dec  2 15:36:57 2021, max compression
+gzip compressed data, was "dist/donjon-scaffold-0.7.9.tar", last modified: Fri Mar 18 17:38:48 2022, max compression
```

## Comparing `donjon-scaffold-0.7.7.tar` & `donjon-scaffold-0.7.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 oheriveaux  (1001) oheriveaux  (1001)        0 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/
-drwxrwxr-x   0 oheriveaux  (1001) oheriveaux  (1001)        0 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/donjon_scaffold.egg-info/
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)        1 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/donjon_scaffold.egg-info/dependency_links.txt
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)      489 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/donjon_scaffold.egg-info/PKG-INFO
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)      271 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/donjon_scaffold.egg-info/SOURCES.txt
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)        9 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/donjon_scaffold.egg-info/top_level.txt
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)       16 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/donjon_scaffold.egg-info/requires.txt
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)      489 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/PKG-INFO
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)      163 2021-12-02 15:36:56.000000 donjon-scaffold-0.7.7/README.md
--rwxrwxr-x   0 oheriveaux  (1001) oheriveaux  (1001)     1273 2021-12-02 15:36:56.000000 donjon-scaffold-0.7.7/setup.py
-drwxrwxr-x   0 oheriveaux  (1001) oheriveaux  (1001)        0 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/scaffold/
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)    13547 2021-12-02 15:36:56.000000 donjon-scaffold-0.7.7/scaffold/stm32.py
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)    98253 2021-12-02 15:36:56.000000 donjon-scaffold-0.7.7/scaffold/__init__.py
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)    25160 2021-12-02 15:36:56.000000 donjon-scaffold-0.7.7/scaffold/iso7816.py
--rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)       38 2021-12-02 15:36:57.000000 donjon-scaffold-0.7.7/setup.cfg
+drwxrwxr-x   0 oheriveaux  (1001) oheriveaux  (1001)        0 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/
+drwxrwxr-x   0 oheriveaux  (1001) oheriveaux  (1001)        0 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/donjon_scaffold.egg-info/
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)        1 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/donjon_scaffold.egg-info/dependency_links.txt
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)      489 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/donjon_scaffold.egg-info/PKG-INFO
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)      271 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/donjon_scaffold.egg-info/SOURCES.txt
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)        9 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/donjon_scaffold.egg-info/top_level.txt
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)       16 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/donjon_scaffold.egg-info/requires.txt
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)      489 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/PKG-INFO
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)      163 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/README.md
+-rwxrwxr-x   0 oheriveaux  (1001) oheriveaux  (1001)     1273 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/setup.py
+drwxrwxr-x   0 oheriveaux  (1001) oheriveaux  (1001)        0 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/scaffold/
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)    13547 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/scaffold/stm32.py
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)    98746 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/scaffold/__init__.py
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)    26768 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/scaffold/iso7816.py
+-rw-rw-r--   0 oheriveaux  (1001) oheriveaux  (1001)       38 2022-03-18 17:38:48.000000 donjon-scaffold-0.7.9/setup.cfg
```

### Comparing `donjon-scaffold-0.7.7/setup.py` & `donjon-scaffold-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="donjon-scaffold",
-    version="0.7.7",
+    version="0.7.9",
     author="Olivier Heriveaux",
     description="Python3 API for the Scaffold board",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ledger-Donjon/scaffold",
     install_requires=["pyserial", "crcmod"],
     packages=find_packages(),
```

### Comparing `donjon-scaffold-0.7.7/scaffold/stm32.py` & `donjon-scaffold-0.7.9/scaffold/stm32.py`

 * *Files identical despite different names*

### Comparing `donjon-scaffold-0.7.7/scaffold/__init__.py` & `donjon-scaffold-0.7.9/scaffold/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2130,39 +2130,51 @@
             # All writes have been processed, we know the FIFO buffer is empty.
             self.__lazy_fifo_total_size = 0
             self.__lazy_fifo_sizes.clear()
             if last_error is not None:
                 raise last_error
 
     @property
-    def timeout(self):
+    def timeout(self) -> Optional[float]:
         """
-        Timeout in seconds for read and write commands. If set to 0, timeout is
-        disabled.
+        Timeout in seconds for read and write commands. If set to None, timeout
+        is disabled.
         """
         if self.__cache_timeout is None:
             return RuntimeError('Timeout not set yet')
-        return self.__cache_timeout * self.timeout_unit
+        if self.__cache_timeout == 0:
+            return None
+        else:
+            return self.__cache_timeout * self.timeout_unit
 
     @timeout.setter
-    def timeout(self, value):
+    def timeout(self, value: Optional[float]):
         if value is None:
-            value = 0
-        n = int(value / self.timeout_unit)
+            n = 0
+        else:
+            n = max(1, int(value / self.timeout_unit))
         if n != self.__cache_timeout:
             self.__set_timeout_raw(n)  # May throw is n out of range.
             self.__cache_timeout = n  # Must be after set_timeout
 
     def push_timeout(self, value):
         """
         Save previous timeout setting in a stack, and set a new timeout value.
         Call to `pop_timeout` will restore previous timeout value.
+        The new effective timeout will be lower or equal to the current
+        timeout. That is, the timeout cannot be increased, previous defined
+        timeout have higher priority.
 
         :param value: New timeout value, in seconds.
         """
+        if value is None:
+            value = self.timeout
+        else:
+            if self.timeout is not None:
+                value = min(self.timeout, value)
         self.__timeout_stack.append(self.timeout)
         self.timeout = value
 
     def pop_timeout(self):
         """
         Restore timeout setting from stack.
 
@@ -2728,15 +2740,15 @@
             during initialization and keep the configuration set by previous
             sessions.
         """
         # Reset to a default configuration
         # This will perform many writes to registers, so we start a lazy
         # section for maximum speed! (about 7 times faster)
         with self.lazy_section():
-            self.timeout = 0
+            self.timeout = None
             # Sometime we don't want the I/Os to be changed, since it may
             # generate pulses and triggering stuff... Reseting the I/Os is an
             # option.
             if init_ios:
                 self.sig_disconnect_all()
                 self.a0.reset_registers()
                 self.a1.reset_registers()
```

### Comparing `donjon-scaffold-0.7.7/scaffold/iso7816.py` & `donjon-scaffold-0.7.9/scaffold/iso7816.py`

 * *Files 4% similar despite different names*

```diff
@@ -346,15 +346,15 @@
             but user should consider using the :meth:`apdu_str` method instead.
         :param trigger: If 'a' is in this string, trigger is raised after
             ISO-7816 header is sent in T=0, and cleared when the following
             response byte arrives. If 'b' is in this string, trigger is raised
             after data field has been transmitted in T=0, and cleared when the
             next response byte is received. If T=1, both 'a' and 'b' will raise
             trigger after the I-block has been transmitted, and will be cleared
-            when first byte of next block ir received.
+            when first byte of next block is received.
         :raises ValueError: if APDU data is invalid.
         :raises RuntimeError: if the received procedure byte is invalid in T=0,
             or if neither T=0 and T=1 protocols are supported by the card.
         :raises T1RedundancyCodeError: If LRC or CRC is wrong in T=1 protocol.
         :return: Response data, with status word.
         """
         if type(the_apdu) == str:
@@ -448,45 +448,82 @@
         else:
             raise RuntimeError(
                 f'Unexpected procedure byte 0x{procedure_byte:02x} received')
 
     def __apdu_t1(self, the_apdu: bytes, trigger: bool = False) -> bytes:
         """
         Send an APDU to the smartcard and retrieve the response, using T=1
-        protocol.
+        protocol. Transmission supports chaining for both command and response.
 
         :param the_apdu: APDU to be sent.
-        :param trigger: If True, raise trigger on last byte transmission.
+        :param trigger: If True, raise trigger on last byte of last I-block
+            transmission.
         :return: Response data, with status word.
         :raises T1RedundancyCodeError: If LRC or CRC is wrong.
         :raises ProtocolError: If an unpexpected response is received.
         """
-        self.transmit_block(0, (self.t1_ns_tx << 6), the_apdu, trigger)
-        self.t1_ns_tx = (self.t1_ns_tx + 1) % 2  # Increment sequence number
-        block = self.receive_block()
-        # Disable trigger is enabled during transmit_block
-        if trigger:
-            self.iso7816.trigger_long = 0
-        pcb = block[1]
-        if pcb & (1 << 7) == 0:
-            # We received an I-block, as expected.
-            # Check that the sequence number is correct
-            if (pcb >> 6) & 1 != self.t1_ns_rx:
-                raise ProtocolError(
-                    'Incorrect received sequence number in I-block '
-                    + block.hex())
-            self.t1_ns_rx = (self.t1_ns_rx + 1) % 2
-        else:
-            if pcb & (1 << 6) == 0:
+        edc_len_dict = {T1RedundancyCode.LRC: 1, T1RedundancyCode.CRC: 2}
+
+        apdu_remaining = the_apdu
+        while len(apdu_remaining):
+            chunk = apdu_remaining[:254]
+            apdu_remaining = apdu_remaining[254:]
+            has_more = min(1, len(apdu_remaining))
+            enable_trigger = trigger and not has_more
+            # Send I-block
+            self.transmit_block(
+                0, (self.t1_ns_tx << 6) + (has_more << 5), chunk,
+                enable_trigger)
+            # Increment sequence number
+            self.t1_ns_tx = (self.t1_ns_tx + 1) % 2
+            if has_more:
+                # We expect a R-block before sending the next info block
+                block = self.receive_block()
+                pcb = block[1]
+                if pcb & (1 << 7) == 0:  # I-block
+                    raise ProtocolError('Expected R-block, received I-block')
+                elif pcb & (1 << 6) == 0:  # R-block
+                    if pcb & 0x0f == 0:  # Error free acknowledgement
+                        pass
+                    elif pcb & 0x0f == 1:
+                        raise ProtocolError(
+                            'Redundancy code error reported by card')
+                    else:
+                        raise ProtocolError(
+                            'Unspecified error reported by card')
+                else:  # S-block
+                    raise ProtocolError('Expected R-block, received I-block')
+
+        response = bytearray()
+        has_more = True
+        while has_more:
+            block = self.receive_block()
+            if enable_trigger:
+                self.iso7816.trigger_long = 0
+            pcb = block[1]
+            if pcb & (1 << 7) == 0:  # I-block
+                # Check that the sequence number is correct
+                if (pcb >> 6) & 1 != self.t1_ns_rx:
+                    raise ProtocolError(
+                        'Incorrect received sequence number in I-block '
+                        + block.hex())
+                has_more = bool((pcb >> 5) & 1)
+                edc_len = edc_len_dict[self.t1_redundancy_code]
+                response += block[3:-edc_len]  # Trim header and EDC
+            elif pcb & (1 << 6) == 0:  # R-block
                 raise ProtocolError('Expected I-block, received R-block')
-            else:
+            else:  # S-block
                 raise ProtocolError('Expected I-block, received S-block')
-        edc_len = {T1RedundancyCode.LRC: 1, T1RedundancyCode.CRC: 2}[
-            self.t1_redundancy_code]
-        return block[3:-edc_len]  # Trim header and EDC
+
+            self.t1_ns_rx = (self.t1_ns_rx + 1) % 2
+            if has_more:
+                # Send R block
+                self.transmit_block(0, 0b10000000 + (self.t1_ns_rx << 4), b'')
+
+        return response
 
     def pps(self, pps1: int) -> int:
         """
         Send a PPS request to change the communication speed parameters Fi and
         Di (as specified in ISO-7816-3). PPS0 and PPS1 are sent. PPS2 is
         ignored. This method waits for the response of the card and then
         automatically changes the ETU from the Fi and Di values.
```


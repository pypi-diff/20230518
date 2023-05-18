# Comparing `tmp/pyopslib-0.0.3.tar.gz` & `tmp/pyopslib-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopslib-0.0.3.tar", max compression
+gzip compressed data, was "pyopslib-0.1.tar", max compression
```

## Comparing `pyopslib-0.0.3.tar` & `pyopslib-0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     2853 2023-03-24 12:40:51.434593 pyopslib-0.0.3/Readme.md
--rw-r--r--   0        0        0     6888 2023-03-31 11:24:46.441580 pyopslib-0.0.3/opslib/ansible.py
--rw-r--r--   0        0        0      648 2023-03-25 14:45:14.773127 pyopslib-0.0.3/opslib/callbacks.py
--rw-r--r--   0        0        0     4258 2023-04-10 17:49:10.777498 pyopslib-0.0.3/opslib/cli.py
--rw-r--r--   0        0        0     3568 2023-04-06 17:36:30.708665 pyopslib-0.0.3/opslib/components.py
--rw-r--r--   0        0        0     1940 2023-04-21 12:01:21.910079 pyopslib-0.0.3/opslib/extras/http.py
--rw-r--r--   0        0        0     3285 2023-04-12 19:01:51.934605 pyopslib-0.0.3/opslib/extras/restic.py
--rw-r--r--   0        0        0     3464 2023-03-26 14:10:06.150347 pyopslib-0.0.3/opslib/extras/systemd.py
--rw-r--r--   0        0        0     3511 2023-04-02 17:35:28.524145 pyopslib-0.0.3/opslib/extras/tailscale.py
--rw-r--r--   0        0        0     1733 2023-04-09 18:41:39.319970 pyopslib-0.0.3/opslib/lazy.py
--rw-r--r--   0        0        0     3279 2023-03-31 11:24:46.442621 pyopslib-0.0.3/opslib/local.py
--rw-r--r--   0        0        0     6123 2023-03-31 11:24:46.442798 pyopslib-0.0.3/opslib/operations.py
--rw-r--r--   0        0        0    11578 2023-03-31 11:24:46.443089 pyopslib-0.0.3/opslib/places.py
--rw-r--r--   0        0        0     2567 2023-04-05 17:25:24.501390 pyopslib-0.0.3/opslib/props.py
--rw-r--r--   0        0        0     1350 2023-03-31 11:24:46.443434 pyopslib-0.0.3/opslib/results.py
--rw-r--r--   0        0        0     2477 2023-03-29 19:10:27.025773 pyopslib-0.0.3/opslib/state.py
--rw-r--r--   0        0        0     9133 2023-04-21 12:15:18.028724 pyopslib-0.0.3/opslib/terraform.py
--rw-r--r--   0        0        0     1612 2023-04-20 18:49:48.015650 pyopslib-0.0.3/opslib/uptodate.py
--rw-r--r--   0        0        0     1111 2023-03-12 19:51:22.597610 pyopslib-0.0.3/opslib/utils.py
--rw-r--r--   0        0        0      770 2023-04-21 12:21:21.316646 pyopslib-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 pyopslib-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3798 2023-05-18 14:28:47.573798 pyopslib-0.1/Readme.md
+-rw-r--r--   0        0        0      230 2023-05-08 19:20:46.729317 pyopslib-0.1/opslib/__init__.py
+-rw-r--r--   0        0        0     6785 2023-05-08 19:20:46.729557 pyopslib-0.1/opslib/ansible.py
+-rw-r--r--   0        0        0      648 2023-05-03 04:12:42.403285 pyopslib-0.1/opslib/callbacks.py
+-rw-r--r--   0        0        0     5370 2023-05-18 12:10:04.698767 pyopslib-0.1/opslib/cli.py
+-rw-r--r--   0        0        0     3269 2023-05-18 13:53:42.087113 pyopslib-0.1/opslib/components.py
+-rw-r--r--   0        0        0     1940 2023-04-21 12:01:21.910079 pyopslib-0.1/opslib/extras/http.py
+-rw-r--r--   0        0        0     3061 2023-05-10 19:21:02.610249 pyopslib-0.1/opslib/extras/restic.py
+-rw-r--r--   0        0        0     3244 2023-05-18 12:10:04.699387 pyopslib-0.1/opslib/extras/systemd.py
+-rw-r--r--   0        0        0     3301 2023-05-10 19:21:02.611000 pyopslib-0.1/opslib/extras/tailscale.py
+-rw-r--r--   0        0        0     1733 2023-04-09 18:41:39.319970 pyopslib-0.1/opslib/lazy.py
+-rw-r--r--   0        0        0     3279 2023-03-31 11:24:46.442621 pyopslib-0.1/opslib/local.py
+-rw-r--r--   0        0        0     6123 2023-05-18 12:10:04.699688 pyopslib-0.1/opslib/operations.py
+-rw-r--r--   0        0        0    13261 2023-05-18 13:53:42.087468 pyopslib-0.1/opslib/places.py
+-rw-r--r--   0        0        0     2567 2023-04-05 17:25:24.501390 pyopslib-0.1/opslib/props.py
+-rw-r--r--   0        0        0     1350 2023-03-31 11:24:46.443434 pyopslib-0.1/opslib/results.py
+-rw-r--r--   0        0        0     1976 2023-05-08 19:20:46.730392 pyopslib-0.1/opslib/state.py
+-rw-r--r--   0        0        0     9183 2023-05-10 19:21:02.611513 pyopslib-0.1/opslib/terraform.py
+-rw-r--r--   0        0        0     1842 2023-05-07 07:52:02.980580 pyopslib-0.1/opslib/uptodate.py
+-rw-r--r--   0        0        0     1111 2023-05-09 07:11:39.237442 pyopslib-0.1/opslib/utils.py
+-rw-r--r--   0        0        0      826 2023-05-18 14:29:43.612730 pyopslib-0.1/pyproject.toml
+-rw-r--r--   0        0        0     4451 1970-01-01 00:00:00.000000 pyopslib-0.1/PKG-INFO
```

### Comparing `pyopslib-0.0.3/opslib/ansible.py` & `pyopslib-0.1/opslib/ansible.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ansible.playbook.play import Play
 from ansible.plugins.callback import CallbackBase
 from ansible.vars.manager import VariableManager
 
 from .callbacks import Callbacks
 from .components import Component
 from .lazy import evaluate
+from .places import BaseHost
 from .props import Prop
 from .results import Result
 from .uptodate import UpToDate
 
 logger = logging.getLogger(__name__)
 
 
@@ -145,30 +146,28 @@
     return result
 
 
 class AnsibleAction(Component):
     """
     The AnsibleAction component executes an Ansible module.
 
-    :param hostname: Name of the host to act on. May be :class:`~opslib.lazy.Lazy`.
-    :param ansible_variables: List of variables to configure Ansible.
+    :param host: :class:`~opslib.places.BaseHost` to act on.
     :param module: Name of the Ansible module to invoke, e.g.
                    ``"ansible.builtin.copy"``.
     :param args: Dictionary of arguments for the module. Consult each module's
                  documentation for the args (or *Parameters*) it supports.
     :param format_output: Optional callback used to format the result output.
                           If provided, it will be called with a single
                           parameter, the :class:`AnsibleResult` object; its
                           return value will be used to overwrite the ``output``
                           attribute of the result.
     """
 
     class Props:
-        hostname = Prop(str, lazy=True)
-        ansible_variables = Prop(list)
+        host = Prop(BaseHost)
         module = Prop(str)
         args = Prop(dict)
         format_output = Prop(Optional[Callable])
 
     uptodate = UpToDate()
     on_change = Callbacks()
 
@@ -178,16 +177,16 @@
             module=self.props.module,
             args=evaluate(self.props.args),
         )
 
     @uptodate.snapshot
     def _get_ansible_args(self):
         return dict(
-            hostname=evaluate(self.props.hostname),
-            ansible_variables=self.props.ansible_variables,
+            hostname=evaluate(self.props.host.hostname),
+            ansible_variables=self.props.host.ansible_variables,
             action=self.action,
         )
 
     def run(self, check=False):
         """
         Call :func:`run_ansible` with the action defined by this component.
         """
```

### Comparing `pyopslib-0.0.3/opslib/callbacks.py` & `pyopslib-0.1/opslib/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyopslib-0.0.3/opslib/cli.py` & `pyopslib-0.1/opslib/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import logging
 import os
 import pdb
 import sys
 
 import click
 
-from .components import init_statedir
 from .operations import apply, print_report
 
 logger = logging.getLogger(__name__)
 
 
 def lookup(component, path):
     for name in path.split("."):
@@ -41,46 +40,78 @@
 
     except ImportError:
         pass
 
     code.interact(banner=banner, local=local)
 
 
+class ComponentGroup(click.Group):
+    def forward_command(self, *args, **kwargs):
+        """
+        A specialized :meth:`click.Group.command` for commands that invoke
+        another command. Any unprocessed arguments are sent as an ``args``
+        tuple, to be forwarded to the other command. It's equivalent to the
+        following:
+
+        .. code-block:: python
+
+            @cli.command(
+                context_settings=dict(
+                    ignore_unknown_options=True,
+                    allow_interspersed_args=False,
+                )
+            )
+            @click.argument("args", nargs=-1, type=click.UNPROCESSED)
+            def foo(args):
+                print("foo called with:", args)
+        """
+
+        func = None
+        if len(args) == 1 and not kwargs and callable(args[0]):
+            func = args[0]
+            args = ()
+
+        def decorator(func):
+            kwargs.setdefault("context_settings", {}).update(
+                ignore_unknown_options=True,
+                allow_interspersed_args=False,
+            )
+            command = super(ComponentGroup, self).command(*args, **kwargs)(func)
+            command.params.append(
+                click.Argument(("args",), nargs=-1, type=click.UNPROCESSED)
+            )
+            return command
+
+        if func:
+            return decorator(func)
+
+        return decorator
+
+
 def get_cli(component):
-    @click.group()
+    @click.group(cls=ComponentGroup)
     def cli():
         pass
 
-    @cli.command("init")
-    def init():
-        init_statedir(component)
-
     @cli.command()
     def id():
         click.echo(repr(component))
 
     @cli.command()
     def ls():
         for child in component:
             click.echo(f"{child._meta.name}: {child!r}")
 
     @cli.command()
     def shell():
         return interact(str(component), dict(self=component))
 
-    @cli.command(
-        "component",
-        context_settings=dict(
-            ignore_unknown_options=True,
-            allow_interspersed_args=False,
-        ),
-    )
+    @cli.forward_command("component")
     @click.pass_context
     @click.argument("path")
-    @click.argument("args", nargs=-1, type=click.UNPROCESSED)
     def component_(ctx, path, args):
         target = lookup(component, path)
         target_cli = get_cli(target)
         target_cli(obj=ctx.obj, args=args)
 
     def register_apply_command(name, *decorators, **defaults):
         @click.pass_context
@@ -158,21 +189,25 @@
                 sys.exit(1)
 
             raise
 
     return cli
 
 
+def get_stack():
+    sys.path.append(os.getcwd())
+    module = importlib.import_module(os.environ.get("OPSLIB_STACK", "stack"))
+    return module.stack
+
+
 def main():
     """
     Main entry point for the ``opslib`` CLI command. It tries to run ``import
-    stack`` and expects to find a callable named ``stack.get_stack``, which it
-    sends to :func:`get_main_cli`.
+    stack`` and expects to find a stack named ``stack.stack``, which it sends
+    to :func:`get_main_cli`.
 
     The ``OPSLIB_STACK`` environment variable can be set to import something
     other than ``stack``.
     """
 
-    sys.path.append(os.getcwd())
-    module = importlib.import_module(os.environ.get("OPSLIB_STACK", "stack"))
-    cli = get_main_cli(module.get_stack)
+    cli = get_main_cli(get_stack)
     cli()
```

### Comparing `pyopslib-0.0.3/opslib/components.py` & `pyopslib-0.1/opslib/components.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import logging
+import sys
 from functools import cached_property
+from pathlib import Path
 
 from .props import InstanceProps
-from .state import StateDirectory, default_state_directory
+from .state import StateDirectory
 
 logger = logging.getLogger(__name__)
 
 
 class Meta:
     statedir = StateDirectory()
 
-    def __init__(self, component, name, parent):
+    def __init__(self, component, name, parent, stateroot=None):
         self.component = component
         self.name = name
         self.parent = parent
+        self.stateroot = stateroot
 
     @cached_property
     def full_name(self):
         if self.parent is None or self.parent._meta.parent is None:
             return self.name
 
         return f"{self.parent._meta.full_name}.{self.name}"
@@ -79,53 +82,42 @@
         """
 
     def add_commands(self, cli):
         """
         Called when the CLI is constructed. Override this method to add custom
         commands.
 
-        :param cli: A :class:`click.Group` that represents the CLI of this
-                    component.
+        :param cli: A :class:`~opslib.cli.ComponentGroup` that represents the
+                    CLI of this component.
         """
 
 
+def get_stateroot(import_name):
+    module = sys.modules[import_name]
+    return Path(module.__file__).parent / ".opslib"
+
+
 class Stack(Component):
-    """
-    Stack represents the root of the component stack. It behaves like a regular
-    :class:`Component`, except that its ``build()`` method is called when it's
-    instantiated.
-    """
+    def __init__(self, import_name=None, stateroot=None, **kwargs):
+        if import_name is None and stateroot is None:
+            raise ValueError("Either `import_name` or `stateroot` must be set")
 
-    def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self._meta = self.Meta(component=self, name="__root__", parent=None)
-        self.build()
 
-    def get_state_directory(self):
-        """
-        Returns the directory where opslib will keep its state. Defaults to a
-        directory named ``.opslib`` in the parent folder of the file where the
-        class is defined. Override this method if you want to store state
-        elsewhere.
-        """
-
-        return default_state_directory(self)
+        self._meta = self.Meta(
+            component=self,
+            name="__root__",
+            parent=None,
+            stateroot=stateroot or get_stateroot(import_name),
+        )
+        self.build()
 
 
 def walk(component):
     """
     Iterate depth-first over all child components. The first item is
     ``component`` itself.
     """
 
     yield component
     for child in component:
         yield from walk(child)
-
-
-def init_statedir(stack):
-    from .operations import Printer
-
-    for component in walk(stack):
-        changed = component._meta.statedir.init()
-        if changed:
-            Printer(component).print_component(changed=True)
```

### Comparing `pyopslib-0.0.3/opslib/extras/http.py` & `pyopslib-0.1/opslib/extras/http.py`

 * *Files identical despite different names*

### Comparing `pyopslib-0.0.3/opslib/extras/restic.py` & `pyopslib-0.1/opslib/extras/restic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from io import StringIO
 from shlex import quote
 
-import click
-
 from opslib.components import Component
 from opslib.lazy import Lazy, evaluate, lazy_property
 from opslib.local import run
 from opslib.props import Prop
 from opslib.results import OperationError, Result
 from opslib.state import JsonState
 
@@ -67,21 +65,15 @@
     def initialized(self):
         return self.state.get("initialized")
 
     def plan(self, **props):
         return ResticPlan(repository=self, **props)
 
     def add_commands(self, cli):
-        @cli.command(
-            context_settings=dict(
-                ignore_unknown_options=True,
-                allow_interspersed_args=False,
-            )
-        )
-        @click.argument("args", nargs=-1, type=click.UNPROCESSED)
+        @cli.forward_command
         def run(args):
             self.run(*args, capture_output=False, exit=True)
 
 
 class ResticPlan(Component):
     class Props:
         repository = Prop(ResticRepository)
```

### Comparing `pyopslib-0.0.3/opslib/extras/systemd.py` & `pyopslib-0.1/opslib/extras/systemd.py`

 * *Files 23% similar despite different names*

```diff
@@ -45,29 +45,27 @@
     def start_command(self):
         return self.props.host.command(
             args=["systemctl", "start", self.props.name],
             run_after=[self.unit_file],
         )
 
     def add_commands(self, cli):
-        @cli.command(context_settings=dict(ignore_unknown_options=True))
+        @cli.forward_command
         @click.argument("command")
-        @click.argument("args", nargs=-1, type=click.UNPROCESSED)
         def systemctl(command, args):
             self.props.host.run(
                 "systemctl",
                 command,
                 self.props.name,
                 *args,
                 capture_output=False,
                 exit=True,
             )
 
-        @cli.command(context_settings=dict(ignore_unknown_options=True))
-        @click.argument("args", nargs=-1, type=click.UNPROCESSED)
+        @cli.forward_command
         def journalctl(args):
             self.props.host.run(
                 "journalctl", "-u", self.props.name, *args, capture_output=False
             )
 
 
 class SystemdTimerService(Component):
```

### Comparing `pyopslib-0.0.3/opslib/extras/tailscale.py` & `pyopslib-0.1/opslib/extras/tailscale.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,16 +118,10 @@
         return json.loads(status_json)["Self"]["ID"] or None
 
     @property
     def node_id(self):
         return self.state.get("node_id")
 
     def add_commands(self, cli):
-        @cli.command(
-            context_settings=dict(
-                ignore_unknown_options=True,
-                allow_interspersed_args=False,
-            )
-        )
-        @click.argument("args", nargs=-1, type=click.UNPROCESSED)
+        @cli.forward_command
         def run(args):
             self.props.run("tailscale", *args, capture_output=False, exit=True)
```

### Comparing `pyopslib-0.0.3/opslib/lazy.py` & `pyopslib-0.1/opslib/lazy.py`

 * *Files identical despite different names*

### Comparing `pyopslib-0.0.3/opslib/local.py` & `pyopslib-0.1/opslib/local.py`

 * *Files identical despite different names*

### Comparing `pyopslib-0.0.3/opslib/operations.py` & `pyopslib-0.1/opslib/operations.py`

 * *Files identical despite different names*

### Comparing `pyopslib-0.0.3/opslib/places.py` & `pyopslib-0.1/opslib/places.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
+import shlex
 import sys
 from copy import copy
 from pathlib import Path
 from typing import Optional, Union
 
-from .ansible import AnsibleAction
 from .callbacks import Callbacks
 from .components import Component
 from .lazy import Lazy, evaluate
 from .local import run
 from .props import Prop
 from .results import Result
 from .state import JsonState
 from .utils import diff
 
 
-class BaseHost:
+class BaseHost(Component):
     """
-    Abstract class for a host.
+    Abstract component for a host.
     """
 
     with_sudo = False
 
     def file(self, **props):
         """
         Shorthand function that returns a :class:`File` component with ``host``
@@ -62,17 +62,18 @@
         """
         Shorthand function that returns an
         :class:`~opslib.ansible.AnsibleAction` component with ``hostname`` and
         ``ansible_variables`` set from this host. Keyword arguments are
         forwarded as props to *AnsibleAction*.
         """
 
+        from .ansible import AnsibleAction
+
         return AnsibleAction(
-            hostname=self.hostname,
-            ansible_variables=self.ansible_variables,
+            host=self,
             **props,
         )
 
     def sudo(self):
         """
         Returns a copy of this host that has the ``with_sudo`` flag set. This
         means that commands will be run using ``sudo``, and Ansible will be
@@ -85,18 +86,23 @@
             *rv.ansible_variables,
             ("ansible_become", "yes"),
             ("ansible_become_method", "sudo"),
             ("ansible_become_user", "root"),
         ]
         return rv
 
+    def add_commands(self, cli):
+        @cli.forward_command
+        def run(args):
+            self.run(*args, capture_output=False, exit=True)
+
 
 class LocalHost(BaseHost):
     """
-    The local host on which opslib is running. It receives no arguments.
+    The local host on which opslib is running. It receives no props.
 
     :ivar hostname: Set to ``localhost``.
     :ivar ansible_variables: Two variables are set: ``ansible_connection`` is
                              ``local``; ``ansible_python_interpreter`` is set
                              to :obj:`sys.executable`.
     """
 
@@ -118,15 +124,15 @@
             shell = os.environ.get("SHELL", "sh")
             args = [shell]
         return run(*args, **kwargs)
 
 
 class SshHost(BaseHost):
     """
-    Connect to a remote host over SSH. Most arguments configure how the ``ssh``
+    Connect to a remote host over SSH. Most props configure how the ``ssh``
     subcommand is invoked. If you have already configured the host in
     ``~/.ssh/config``, it's enough to specify ``hostname``, as you would in the
     terminal.
 
     :param hostname: Name of the remote host.
     :param username: Username to log in.
     :param port: Port number.
@@ -135,72 +141,79 @@
     :param config_file: SSH configuration file to use instead of
                         ``~/.ssh/config``.
     :param interpreter: Python interpreter to be used by Ansible. Set as the
                         ``ansible_python_interpreter`` variable. Defaults to
                         ``"python3"``.
     """
 
-    def __init__(
-        self,
-        hostname,
-        username=None,
-        port=None,
-        private_key_file=None,
-        config_file=None,
-        interpreter="python3",
-    ):
-        self.hostname = hostname
-        self.port = port
-        self.username = username
-        self.private_key_file = private_key_file
-        self.config_file = config_file
+    class Props:
+        hostname = Prop(str, lazy=True)
+        username = Prop(Optional[str])
+        port = Prop(Optional[int])
+        private_key_file = Prop(Optional[Path])
+        config_file = Prop(Optional[Path])
+        interpreter = Prop(str, default="python3")
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)  # TODO always attach host to stack
         self.ansible_variables = [
-            ("ansible_python_interpreter", interpreter),
+            ("ansible_python_interpreter", self.props.interpreter),
         ]
 
-        if port:
-            self.ansible_variables.append(("ansible_ssh_port", str(port)))
+        if self.props.port:
+            self.ansible_variables.append(("ansible_ssh_port", str(self.props.port)))
 
-        if username:
-            self.ansible_variables.append(("ansible_user", username))
+        if self.props.username:
+            self.ansible_variables.append(("ansible_user", self.props.username))
 
-        if private_key_file:
+        if self.props.private_key_file:
             self.ansible_variables.append(
-                ("ansible_ssh_private_key_file", str(private_key_file))
+                ("ansible_ssh_private_key_file", str(self.props.private_key_file))
             )
 
-        if config_file:
+        if self.props.config_file:
             self.ansible_variables.append(
-                ("ansible_ssh_common_args", f"-F {config_file}"),
+                ("ansible_ssh_common_args", f"-F {self.props.config_file}"),
             )
 
+    @property
+    def hostname(self):
+        return self.props.hostname
+
     def run(self, *args, **kwargs):
         """
         Run a command on the remote host.
 
         It uses :func:`~opslib.local.run` to invoke ``ssh`` with the given
         arguments.
         """
 
         hostname = evaluate(self.hostname)
-        if self.username:
-            hostname = f"{self.username}@{hostname}"
+        if self.props.username:
+            hostname = f"{self.props.username}@{hostname}"
 
         ssh_args = ["ssh", hostname]
-        if self.port:
-            ssh_args += ["-p", str(self.port)]
+        if self.props.port:
+            ssh_args += ["-p", str(self.props.port)]
 
-        if self.private_key_file:
-            ssh_args += ["-i", str(self.private_key_file)]
+        if self.props.private_key_file:
+            ssh_args += ["-i", str(self.props.private_key_file)]
 
-        if self.config_file:
-            ssh_args += ["-F", str(self.config_file)]
+        if self.props.config_file:
+            ssh_args += ["-F", str(self.props.config_file)]
 
         ssh_args.append("--")
 
+        cwd = kwargs.pop("cwd", None)
+        if cwd is not None:
+            cwd = str(cwd)
+            if cwd != shlex.quote(cwd):
+                raise ValueError("CWD must not contain special characters")
+            ssh_args += ["cd", cwd, "&&"]
+
         if self.with_sudo:
             ssh_args.append("sudo")
             if not args:
                 args = ["-i"]
 
         return run(*ssh_args, *args, **kwargs)
 
@@ -252,20 +265,27 @@
         self.action = self.host.ansible_action(
             module="ansible.builtin.copy",
             args=args,
             format_output=self.format_output,
         )
 
     def format_output(self, result):
+        diffs = []
+
         if result.changed:
-            return "".join(
-                diff(self.path, d["before"], d["after"]) for d in result.data["diff"]
-            )
+            data_diff = result.data["diff"]
+            if isinstance(data_diff, dict):
+                before = f'{data_diff["before"]}\n'
+                after = f'{data_diff["after"]}\n'
+                diffs.append(diff(self.path, before, after))
+
+            else:
+                diffs += [diff(self.path, d["before"], d["after"]) for d in data_diff]
 
-        return ""
+        return "".join(diffs)
 
     @property
     def on_change(self):
         return self.action.on_change
 
 
 class Directory(Component):
@@ -341,33 +361,58 @@
 
         return File(
             host=self.host,
             path=self.path / name,
             **kwargs,
         )
 
+    def command(self, **props):
+        """
+        Shorthand function that returns a :class:`Command` component with
+        ``cwd`` set to this directory and ``host`` set to this host. Keyword
+        arguments are forwarded as props to the Command.
+        """
+
+        return Command(
+            host=self.host,
+            cwd=self.path,
+            **props,
+        )
+
+    def run(self, *args, **kwargs):
+        """
+        Run a command inside this directory. If ``args`` is empty, it defaults
+        to a single argument, ``$SHELL``.
+
+        It invokes :func:`~opslib.local.run` with the arguments.
+        """
+
+        return self.host.run(cwd=self.path, *args, **kwargs)
+
 
 class Command(Component):
     """
     The Command component represents a command that should be run on the
     host during deployment.
 
     :param host: The parent host.
+    :param cwd: Optional :class:`~pathlib.Path` where command should run.
     :param args: Command arguments array. The first argument is the command
                  itself. Defaults to ``[]``, which invokes the shell, useful
                  with the ``input`` parameter.
     :param input: Content to be sent to standard input. Defaults to no input.
     :param run_after: A list of components that trigger this command to be run.
                       If empty, the command will always be run, otherwise it
                       will run once, and then only run after one of the
                       components changes.
     """
 
     class Props:
         host = Prop(BaseHost)
+        cwd = Prop(Optional[Path])
         args = Prop(Union[list, tuple], default=[])
         input = Prop(Optional[str])
         run_after = Prop(list, default=[])
 
     state = JsonState()
     on_change = Callbacks()
 
@@ -384,14 +429,15 @@
 
         :param kwargs: Extra keyword arguments to be forwarded to the ``run``
                        method of the host.
         """
 
         return self.host.run(
             *self.props.args,
+            cwd=self.props.cwd,
             input=self.props.input,
             **kwargs,
         )
 
     def build(self):
         for other in self.props.run_after:
             other.on_change.add(self._set_must_run)
```

### Comparing `pyopslib-0.0.3/opslib/props.py` & `pyopslib-0.1/opslib/props.py`

 * *Files identical despite different names*

### Comparing `pyopslib-0.0.3/opslib/results.py` & `pyopslib-0.1/opslib/results.py`

 * *Files identical despite different names*

### Comparing `pyopslib-0.0.3/opslib/state.py` & `pyopslib-0.1/opslib/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,55 @@
 import json
 import logging
-import sys
-from functools import cached_property
-from pathlib import Path
 
 logger = logging.getLogger(__name__)
 
 
 class ComponentStateDirectory:
     def __init__(self, meta):
         self.meta = meta
 
-        if meta.parent is None:
-            self._prefix = meta.component.get_state_directory()
+    @property
+    def prefix(self):
+        if self.meta.parent is None:
+            prefix = self.meta.stateroot
 
         else:
-            self._prefix = meta.parent._meta.statedir._prefix / meta.name
+            parent_meta = self.meta.parent._meta
+            prefix = parent_meta.statedir.prefix / self.meta.name
 
-        self._path = self._prefix / "_statedir"
+        self._mkdir(prefix)
+        return prefix
 
-    def init(self):
-        changed = False
-
-        if not self._prefix.exists():
-            logger.debug("ComponentState init %s", self._prefix)
-            self._prefix.mkdir(mode=0o700)
-            changed = True
-
-        if not self._path.exists():
-            logger.debug("ComponentState init %s", self._path)
-            self._path.mkdir(mode=0o700)
-            changed = True
-
-        return changed
-
-    @cached_property
+    @property
     def path(self):
-        assert (
-            self._path.is_dir()
-        ), f"State directory for {self.meta.component!r} missing, please run `init`."
-        return self._path
+        path = self.prefix / "_statedir"
+        self._mkdir(path)
+        return path
+
+    def _mkdir(self, path):
+        if not path.is_dir():
+            logger.debug("ComponentState init %s", path)
+            path.mkdir(mode=0o700)
 
 
 class StateDirectory:
     def __get__(self, obj, objtype=None):
         return ComponentStateDirectory(obj)
 
 
-def default_state_directory(stack):
-    module = sys.modules[stack.__module__]
-    return Path(module.__file__).parent / ".opslib"
-
-
 class ComponentJsonState:
     def __init__(self, component):
         self.component = component
 
-    @cached_property
+    @property
     def _path(self):
         return self.component._meta.statedir.path / "state.json"
 
-    @cached_property
+    @property
     def _data(self):
         try:
             with self._path.open() as f:
                 return json.load(f)
 
         except FileNotFoundError:
             return {}
```

### Comparing `pyopslib-0.0.3/opslib/terraform.py` & `pyopslib-0.1/opslib/terraform.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import json
 import os
 from functools import cached_property
 from typing import Optional
 
-import click
-
 from .components import Component
 from .lazy import Lazy, NotAvailable, evaluate
 from .local import run
 from .props import Prop
 from .results import Result
 from .uptodate import UpToDate
 
@@ -59,24 +57,24 @@
 
     @cached_property
     def plugin_cache_path(self):
         return self._meta.statedir.path / "plugin-cache"
 
     @cached_property
     def config(self):
-        provider_body = dict()
+        provider_args = dict()
         if self.props.source:
-            provider_body["source"] = self.props.source
+            provider_args["source"] = self.props.source
         if self.props.version:
-            provider_body["version"] = self.props.version
+            provider_args["version"] = self.props.version
 
         config = dict(
             terraform=dict(
                 required_providers={
-                    self.props.name: provider_body,
+                    self.props.name: provider_args,
                 },
             ),
         )
 
         if self.props.config:
             config["provider"] = {self.props.name: self.props.config}
 
@@ -105,15 +103,15 @@
         )
 
 
 class _TerraformComponent(Component):
     class Props:
         provider = Prop(Optional[TerraformProvider])
         type = Prop(str)
-        body = Prop(dict, default={}, lazy=True)
+        args = Prop(dict, default={}, lazy=True)
         output = Prop(Optional[list])
 
     @cached_property
     def tf_path(self):
         return self._meta.statedir.path / "terraform"
 
     def _run(self, *args, **kwargs):
@@ -163,35 +161,29 @@
                 return output["value"]
 
             return Lazy(get_value)
 
         return {name: lazy_output(name) for name in self.props.output}
 
     def add_commands(self, cli):
-        @cli.command(
-            context_settings=dict(
-                ignore_unknown_options=True,
-                allow_interspersed_args=False,
-            )
-        )
-        @click.argument("args", nargs=-1, type=click.UNPROCESSED)
+        @cli.forward_command
         def terraform(args):
             self.run(*args, capture_output=False, exit=True)
 
 
 class TerraformResource(_TerraformComponent):
     """
     The TerraformResource component creates a single Resource through
     Terraform.
 
     :param provider: The :class:`TerraformProvider` for this resource.
                      Technically optional because some builtin resource types
                      of Terraform don't belong to any provider.
     :param type: Type of resource, e.g. ``"aws_vpc"``.
-    :param body: Arguments of the resource (:class:`dict`). Consult the
+    :param args: Arguments of the resource (:class:`dict`). Consult the
                  provider's documentation for the arguments supported by each
                  resource. May be :class:`~opslib.lazy.Lazy`.
     :param output: List of attributes exported by the resource to be fetched
                    from Terraform. They are available on the ``output``
                    property. (optional)
     """
 
@@ -201,15 +193,15 @@
     @uptodate.snapshot
     def config(self):
         provider = self.props.provider
         config = dict(
             provider.config if provider else {},
             resource={
                 self.props.type: {
-                    "thing": evaluate(self.props.body),
+                    "thing": evaluate(self.props.args),
                 },
             },
         )
 
         if self.props.output:
             config["output"] = {
                 key: {
@@ -222,37 +214,46 @@
         return config
 
     @uptodate.refresh
     def refresh(self):
         self.run("refresh")
         return TerraformResult(self.run("plan"))
 
-    @uptodate.deploy
-    def deploy(self, dry_run=False):
+    def _apply(self, dry_run=False, destroy=False):
         args = ["plan"] if dry_run else ["apply", "-auto-approve"]
+        if destroy:
+            args.append("-destroy")
         return TerraformResult(self.run(*args, "-refresh=false"))
 
+    @uptodate.deploy
+    def deploy(self, dry_run=False):
+        return self._apply(dry_run=dry_run)
+
+    @uptodate.destroy
+    def destroy(self, dry_run=False):
+        return self._apply(dry_run=dry_run, destroy=True)
+
     def import_resource(self, resource_id):
         """
         Import an existing resource into Terraform.
         """
 
         return self.run("import", f"{self.props.type}.thing", evaluate(resource_id))
 
 
-class TerraformDataSource(TerraformResource):
+class TerraformDataSource(_TerraformComponent):
     """
     The TerraformDataSource component retrieves data through a Terraform data
     source.
 
     :param provider: The :class:`TerraformProvider` for this data source.
                      Technically optional because some builtin data source
                      types of Terraform don't belong to any provider.
     :param type: Type of data source, e.g. ``"aws_vpc"``.
-    :param body: Arguments of the data source (:class:`dict`). Consult the
+    :param args: Arguments of the data source (:class:`dict`). Consult the
                  provider's documentation for the arguments supported by each
                  data source. May be :class:`~opslib.lazy.Lazy`.
     :param output: List of attributes exported by the data source to be fetched
                    from Terraform. They are available on the ``output``
                    property. (optional)
     """
 
@@ -262,15 +263,15 @@
     @uptodate.snapshot
     def config(self):
         provider = self.props.provider
         config = dict(
             provider.config if provider else {},
             data={
                 self.props.type: {
-                    "thing": evaluate(self.props.body),
+                    "thing": evaluate(self.props.args),
                 },
             },
         )
 
         if self.props.output:
             config["output"] = {
                 key: {
```

### Comparing `pyopslib-0.0.3/opslib/uptodate.py` & `pyopslib-0.1/opslib/uptodate.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,7 +56,16 @@
                 return Result()
 
             result = func(obj, dry_run=dry_run)
             obj.uptodate.set((not result.changed) if dry_run else True)
             return result
 
         return decorator
+
+    def destroy(self, func):
+        @wraps(func)
+        def decorator(obj, dry_run=False):
+            result = func(obj, dry_run=dry_run)
+            obj.uptodate.set(False)
+            return result
+
+        return decorator
```

### Comparing `pyopslib-0.0.3/opslib/utils.py` & `pyopslib-0.1/opslib/utils.py`

 * *Files identical despite different names*

### Comparing `pyopslib-0.0.3/pyproject.toml` & `pyopslib-0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
+[tool.isort]
+profile = "black"
+
 [tool.poetry]
 name = "pyopslib"
-version = "0.0.3"
+version = "0.1"
 description = "A Pythonic toolkit to manage infrastructure."
 authors = ["Alex Morega <alex@grep.ro>"]
 license = "MIT"
 readme = "Readme.md"
 packages = [
   { include = "opslib" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 beartype = "^0.12.0"
 click = "^8.1.3"
-ansible-core = "^2.14.3"
+ansible-core = "^2.14.3, < 2.15"
 requests = "^2.28.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-black-ng = "^0.4.1"
 pytest-isort = "^3.1.0"
 sphinx = "^6.1.3"
 sphinx-autobuild = "^2021.3.14"
 
 [tool.poetry.scripts]
 opslib = "opslib.cli:main"
 
 [tool.pytest.ini_options]
-addopts = "--black --isort"
+addopts = "--black --isort --ignore examples"
 log_level = "DEBUG"
 markers = [
   "slow: marks tests as slow",
 ]
 
 [build-system]
 requires = ["poetry-core"]
```


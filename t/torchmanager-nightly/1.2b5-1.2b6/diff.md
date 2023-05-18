# Comparing `tmp/torchmanager_nightly-1.2b5.tar.gz` & `tmp/torchmanager_nightly-1.2b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager_nightly-1.2b5.tar", max compression
+gzip compressed data, was "torchmanager_nightly-1.2b6.tar", max compression
```

## Comparing `torchmanager_nightly-1.2b5.tar` & `torchmanager_nightly-1.2b6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1318 2023-04-21 19:45:23.217167 torchmanager_nightly-1.2b5/LICENSE
--rw-r--r--   0        0        0      659 2023-05-11 14:10:04.977471 torchmanager_nightly-1.2b5/pyproject.toml
--rw-r--r--   0        0        0      290 2023-05-08 17:31:19.548937 torchmanager_nightly-1.2b5/torchmanager/__init__.py
--rw-r--r--   0        0        0    10862 2023-05-08 17:31:19.549758 torchmanager_nightly-1.2b5/torchmanager/basic.py
--rw-r--r--   0        0        0      638 2023-05-11 13:57:10.996802 torchmanager_nightly-1.2b5/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4444 2023-05-08 17:31:19.551173 torchmanager_nightly-1.2b5/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4542 2023-05-08 15:41:32.410921 torchmanager_nightly-1.2b5/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3523 2023-05-08 15:41:32.411287 torchmanager_nightly-1.2b5/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1608 2023-05-08 15:41:32.411512 torchmanager_nightly-1.2b5/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4642 2023-05-11 13:57:10.998528 torchmanager_nightly-1.2b5/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2224 2023-05-08 15:41:32.412048 torchmanager_nightly-1.2b5/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2599 2023-05-11 13:57:10.999017 torchmanager_nightly-1.2b5/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      963 2023-05-08 15:41:32.412409 torchmanager_nightly-1.2b5/torchmanager/compatibility.py
--rw-r--r--   0        0        0       26 2023-05-08 17:31:19.551425 torchmanager_nightly-1.2b5/torchmanager/configs/__init__.py
--rw-r--r--   0        0        0     2938 2023-05-08 17:31:19.551828 torchmanager_nightly-1.2b5/torchmanager/configs/basic.py
--rw-r--r--   0        0        0       85 2023-05-08 15:41:32.412717 torchmanager_nightly-1.2b5/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6872 2023-05-08 17:31:19.552543 torchmanager_nightly-1.2b5/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2238 2023-05-08 17:31:19.553192 torchmanager_nightly-1.2b5/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      156 2023-05-08 17:31:19.553780 torchmanager_nightly-1.2b5/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5386 2023-05-08 15:41:32.413797 torchmanager_nightly-1.2b5/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1047 2023-05-08 17:31:19.554805 torchmanager_nightly-1.2b5/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     5757 2023-05-08 17:31:19.555336 torchmanager_nightly-1.2b5/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     3117 2023-05-08 17:31:19.555950 torchmanager_nightly-1.2b5/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      333 2023-05-08 17:31:19.556524 torchmanager_nightly-1.2b5/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     4033 2023-05-08 17:31:19.557449 torchmanager_nightly-1.2b5/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     3678 2023-05-08 17:31:19.558421 torchmanager_nightly-1.2b5/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     5139 2023-05-11 13:57:10.999702 torchmanager_nightly-1.2b5/torchmanager/metrics/extractor.py
--rw-r--r--   0        0        0     2070 2023-05-08 17:31:19.561159 torchmanager_nightly-1.2b5/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4003 2023-05-08 17:31:19.561917 torchmanager_nightly-1.2b5/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     9661 2023-05-08 17:31:19.562736 torchmanager_nightly-1.2b5/torchmanager/testing.py
--rw-r--r--   0        0        0       96 2023-05-08 17:31:19.563726 torchmanager_nightly-1.2b5/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4964 2023-05-08 15:41:32.416190 torchmanager_nightly-1.2b5/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0      694 2023-05-08 17:31:19.564048 torchmanager_nightly-1.2b5/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    14606 2023-05-08 17:31:19.564657 torchmanager_nightly-1.2b5/torchmanager/training.py
--rw-r--r--   0        0        0      459 2023-05-08 17:31:19.565967 torchmanager_nightly-1.2b5/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      109 2023-05-08 17:31:19.566369 torchmanager_nightly-1.2b5/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     4879 2023-05-08 17:31:19.567159 torchmanager_nightly-1.2b5/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-05-08 15:41:32.417827 torchmanager_nightly-1.2b5/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-05-11 13:57:11.006538 torchmanager_nightly-1.2b5/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      350 2023-05-08 15:41:32.418186 torchmanager_nightly-1.2b5/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-05-08 15:41:32.418350 torchmanager_nightly-1.2b5/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     2772 2023-05-08 17:31:19.568914 torchmanager_nightly-1.2b5/torchmanager_core/protocols.py
--rw-r--r--   0        0        0       44 2023-05-08 17:31:19.569189 torchmanager_nightly-1.2b5/torchmanager_core/random/__init__.py
--rw-r--r--   0        0        0     1029 2023-05-08 17:31:19.569753 torchmanager_nightly-1.2b5/torchmanager_core/random/seed.py
--rw-r--r--   0        0        0      204 2023-05-08 15:41:32.418803 torchmanager_nightly-1.2b5/torchmanager_core/typing.py
--rw-r--r--   0        0        0     5137 2023-05-08 17:31:19.570362 torchmanager_nightly-1.2b5/torchmanager_core/version.py
--rw-r--r--   0        0        0      439 2023-05-08 17:31:19.570634 torchmanager_nightly-1.2b5/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-05-08 15:41:32.420108 torchmanager_nightly-1.2b5/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b5/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-04-21 19:45:23.217167 torchmanager_nightly-1.2b6/LICENSE
+-rw-r--r--   0        0        0      659 2023-05-16 17:55:19.687071 torchmanager_nightly-1.2b6/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-05-11 18:30:52.166030 torchmanager_nightly-1.2b6/torchmanager/__init__.py
+-rw-r--r--   0        0        0    10862 2023-05-11 18:30:52.166340 torchmanager_nightly-1.2b6/torchmanager/basic.py
+-rw-r--r--   0        0        0      638 2023-05-11 18:30:52.166882 torchmanager_nightly-1.2b6/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4444 2023-05-11 18:30:52.167385 torchmanager_nightly-1.2b6/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4628 2023-05-11 18:16:52.815262 torchmanager_nightly-1.2b6/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3523 2023-05-11 14:13:25.691390 torchmanager_nightly-1.2b6/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1608 2023-05-11 14:13:25.691561 torchmanager_nightly-1.2b6/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4642 2023-05-11 18:30:52.167957 torchmanager_nightly-1.2b6/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2224 2023-05-11 14:13:25.691701 torchmanager_nightly-1.2b6/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2599 2023-05-11 18:30:52.168441 torchmanager_nightly-1.2b6/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      963 2023-05-11 14:13:25.691910 torchmanager_nightly-1.2b6/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-05-11 18:30:52.168697 torchmanager_nightly-1.2b6/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     2930 2023-05-16 17:55:19.687727 torchmanager_nightly-1.2b6/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-05-11 14:13:25.692993 torchmanager_nightly-1.2b6/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6968 2023-05-11 18:30:52.169618 torchmanager_nightly-1.2b6/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2238 2023-05-11 18:30:52.170275 torchmanager_nightly-1.2b6/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      156 2023-05-11 18:30:52.170737 torchmanager_nightly-1.2b6/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5386 2023-05-11 14:13:25.694420 torchmanager_nightly-1.2b6/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1047 2023-05-11 18:30:52.171245 torchmanager_nightly-1.2b6/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5757 2023-05-11 18:30:52.171684 torchmanager_nightly-1.2b6/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3117 2023-05-11 18:30:52.172126 torchmanager_nightly-1.2b6/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      333 2023-05-11 18:30:52.172601 torchmanager_nightly-1.2b6/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     4033 2023-05-11 18:30:52.173018 torchmanager_nightly-1.2b6/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     3678 2023-05-11 18:30:52.173338 torchmanager_nightly-1.2b6/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5139 2023-05-11 18:30:52.173571 torchmanager_nightly-1.2b6/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2070 2023-05-11 18:30:52.173883 torchmanager_nightly-1.2b6/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4003 2023-05-11 18:30:52.174208 torchmanager_nightly-1.2b6/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     9558 2023-05-16 21:36:19.364793 torchmanager_nightly-1.2b6/torchmanager/testing.py
+-rw-r--r--   0        0        0       96 2023-05-11 18:30:52.175047 torchmanager_nightly-1.2b6/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4964 2023-05-11 14:13:25.700320 torchmanager_nightly-1.2b6/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      694 2023-05-11 18:30:52.175406 torchmanager_nightly-1.2b6/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    14038 2023-05-16 21:36:41.276799 torchmanager_nightly-1.2b6/torchmanager/training.py
+-rw-r--r--   0        0        0      459 2023-05-11 18:30:52.176395 torchmanager_nightly-1.2b6/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-11 18:30:52.176766 torchmanager_nightly-1.2b6/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4879 2023-05-11 18:30:52.177250 torchmanager_nightly-1.2b6/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-05-11 14:13:25.702386 torchmanager_nightly-1.2b6/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-05-11 14:13:30.152271 torchmanager_nightly-1.2b6/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      350 2023-05-11 14:13:25.703024 torchmanager_nightly-1.2b6/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-05-11 14:13:25.703150 torchmanager_nightly-1.2b6/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     2772 2023-05-11 18:30:52.178286 torchmanager_nightly-1.2b6/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-05-11 18:30:52.178624 torchmanager_nightly-1.2b6/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-05-11 18:30:52.178907 torchmanager_nightly-1.2b6/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-05-11 14:13:25.704534 torchmanager_nightly-1.2b6/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     5260 2023-05-16 17:55:19.688600 torchmanager_nightly-1.2b6/torchmanager_core/version.py
+-rw-r--r--   0        0        0      439 2023-05-11 18:30:52.179903 torchmanager_nightly-1.2b6/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-11 14:13:25.706452 torchmanager_nightly-1.2b6/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b6/PKG-INFO
```

### Comparing `torchmanager_nightly-1.2b5/LICENSE` & `torchmanager_nightly-1.2b6/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/pyproject.toml` & `torchmanager_nightly-1.2b6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "torchmanager-nightly"
-version = "1.2b5"
-description = "PyTorch Training Manager v1.2 (Beta 5)"
+version = "1.2b6"
+description = "PyTorch Training Manager v1.2 (Beta 6)"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
```

### Comparing `torchmanager_nightly-1.2b5/torchmanager/basic.py` & `torchmanager_nightly-1.2b6/torchmanager/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/callbacks/__init__.py` & `torchmanager_nightly-1.2b6/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/callbacks/callback.py` & `torchmanager_nightly-1.2b6/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/callbacks/ckpt.py` & `torchmanager_nightly-1.2b6/torchmanager/callbacks/ckpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,39 +13,43 @@
 
     * extends: `.Callback
 
     - Properties:
         - ckpt_path: A `str` of checkpoint path
     """
     __ckpt_path: str
-    _checkpoint: Ckpt[T]
+    __checkpoint: Ckpt[T]
 
     @property
     def ckpt_path(self) -> str:
         return self.__ckpt_path
 
     @ckpt_path.setter
     def ckpt_path(self, p: str) -> None:
         self.__ckpt_path = os.path.normpath(p)
 
+    @property
+    def checkpoint(self) -> Ckpt[T]:
+        return self.__checkpoint
+
     def __init__(self, model: T, ckpt_path: str, **kwargs: Any) -> None:
         """
         Constructor
 
         - Parameters:
             - model: Any type of model to be saved
             - ckpt_path: A `str` of the checkpoint path
             - **kwargs: Other arguments in `Checkpoint` constructor
         """
         super().__init__()
-        self._checkpoint = Ckpt(model, **kwargs)
+        self.__checkpoint = Ckpt(model, **kwargs)
         self.ckpt_path = os.path.normpath(ckpt_path)
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = ...) -> None:
-        self._checkpoint.save(epoch, self.ckpt_path)
+        self.checkpoint.save(epoch, self.ckpt_path)
 
 class LastCheckpoint(_Checkpoint[T]):
     """
     Last checkpoint with frequency control support
 
     * extends: `_Checkpoint`
```

### Comparing `torchmanager_nightly-1.2b5/torchmanager/callbacks/dynamic.py` & `torchmanager_nightly-1.2b6/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/callbacks/early_stop.py` & `torchmanager_nightly-1.2b6/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/callbacks/experiment.py` & `torchmanager_nightly-1.2b6/torchmanager/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/callbacks/lr.py` & `torchmanager_nightly-1.2b6/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/callbacks/tensorboard.py` & `torchmanager_nightly-1.2b6/torchmanager/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/compatibility.py` & `torchmanager_nightly-1.2b6/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/configs/basic.py` & `torchmanager_nightly-1.2b6/torchmanager/configs/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,14 @@
         return configs
 
     @staticmethod
     def get_arguments(parser: Union[argparse.ArgumentParser, argparse._ArgumentGroup] = argparse.ArgumentParser()) -> Union[argparse.ArgumentParser, argparse._ArgumentGroup]:
         parser.add_argument("-exp", "--experiment", type=str, default="test.exp", help="The name of experiment")
         parser.add_argument("--replace_experiment", action="store_true", default=False, help="The flag to replace given experiment if exists.")
         return parser
-    
+
     def show_environments(self) -> None:
         view.logger.info(f"torch={torch.__version__}, torchmanager={VERSION}")
-    
+
     @abc.abstractmethod
     def show_settings(self) -> None:
         pass
```

### Comparing `torchmanager_nightly-1.2b5/torchmanager/data/dataset.py` & `torchmanager_nightly-1.2b6/torchmanager/data/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     * Used as a combination of `torch.utils.data.Dataset` and `torch.utils.data.DataLoader`
 
     >>> from torchmanager import Manager
     >>> class SomeDataset(Dataset):
     ...    @property
     ...    def unbatched_size(self) -> int: ...
     ...
-    ...    def __init__(self, ...,  batch_size: int, device: torch.device = devices.CPU) -> None: ...
     ...    def __getitem__(self, index: Any) -> Any: ...
     >>> dataset = SomeDataset(..., batch_size)
     >>> manager = Manager(...)
     >>> manager.fit(dataset, ...)
 
     - Properties:
         - batch_size: An `int` of batch size for the current dataset
@@ -97,18 +96,17 @@
         return NotImplemented
 
     def __iter__(self) -> Iterator[T]:
         # initialize devices
         cpu_count = os.cpu_count()
         if cpu_count is None:
             cpu_count = 0
-        device = self.device
 
         # initialize loader
-        if device != devices.CPU:
+        if self.device != devices.CPU:
             data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=cpu_count, pin_memory=True, pin_memory_device=str(self.device))
         else:
             data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=cpu_count)
 
         # yield data
         for data in data_loader:
             yield self.unpack_data(data)
@@ -122,18 +120,20 @@
         """
         Unpacks a single data into inputs and targets
 
         - Parameters:
             - data: `Any` kind of single data
         - Returns: `Any` kind of inputs with type `T`
         """
-        if isinstance(data, Sequence):
-            return data[0], data[1] if len(data) >= 2 else NotImplemented # type: ignore
+        if isinstance(data, torch.Tensor) or isinstance(data, dict):
+            return data, data  # type: ignore # suppose for unsupervised reconstruction or a dictionary of packed data
+        if isinstance(data, Sequence) and len(data) == 2:
+            return data[0], data[1]  # type: ignore # suppose for supervised
         else:
-            return NotImplemented
+            return NotImplemented  # unknown type of dataset
 
 
 def batched(fn: Callable[..., _Dataset]):
     """
     Wrap a loading PyTorch dataset function into a loading dataset function
 
     Use as decorator with a function:
```

### Comparing `torchmanager_nightly-1.2b5/torchmanager/data/sliding.py` & `torchmanager_nightly-1.2b6/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/losses/cross_entropy.py` & `torchmanager_nightly-1.2b6/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/losses/dice.py` & `torchmanager_nightly-1.2b6/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/losses/loss.py` & `torchmanager_nightly-1.2b6/torchmanager/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/losses/mse.py` & `torchmanager_nightly-1.2b6/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/metrics/accuracy.py` & `torchmanager_nightly-1.2b6/torchmanager/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/metrics/conf_met.py` & `torchmanager_nightly-1.2b6/torchmanager/metrics/conf_met.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/metrics/extractor.py` & `torchmanager_nightly-1.2b6/torchmanager/metrics/extractor.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/metrics/iou.py` & `torchmanager_nightly-1.2b6/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/metrics/metric.py` & `torchmanager_nightly-1.2b6/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/testing.py` & `torchmanager_nightly-1.2b6/torchmanager/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,44 @@
 
     Testing the model using `test` function:
     >>> from torchmanager.data import Dataset
     >>> dataset = Dataset(...)
     >>> manager.test(dataset, ...)
 
     - Properties:
-        - compiled_losses: The loss function in `Loss` that must be exist
         - compiled_metrics: The `dict` of metrics in `Resulting` that does not contain losses
+        - summary: A `dict` of metrics summary with name in `str` and value in `float`
     """
     model: Union[Module, torch.nn.parallel.DataParallel]
 
     @property
     def compiled_metrics(self) -> Dict[str, Resulting]:
         return {name: m for name, m in self.metric_fns.items() if "loss" not in name}
 
+    @property
+    def summary(self) -> Dict[str, float]:
+        # initialize
+        summary: Dict[str, float] = {}
+
+        # summarize loss
+        if self.loss_fn is not None:
+            summary["loss"] = float(self.loss_fn.result.detach())
+
+        # summarize metrics
+        for name, fn in self.metric_fns.items():
+            if name.startswith("val_"):
+                name = name.replace("val_", "")
+            try:
+                summary[name] = float(fn.result.detach())
+            except Exception as metric_error:
+                runtime_error = errors.MetricError(name)
+                raise runtime_error from metric_error
+        return summary
+
+
     def forward(self, x_train: Any) -> Any:
         """
         Forward pass function
 
         - Parameters:
             - x_train: The training data
         - Returns: `Any` kind of model output
@@ -119,17 +140,14 @@
         """
         # initialize device
         cpu, device, target_devices = devices.search(device)
         if device == cpu and len(target_devices) < 2:
             use_multi_gpus = False
         devices.set_default(target_devices[0])
 
-        # initialize summary
-        summary: Dict[str, float] = {}
-
         # initialize progress bar
         if len(dataset) == 0:
             return {}
         elif isinstance(dataset, Dataset):
             dataset_len = dataset.batched_len
         else:
             dataset_len = len(dataset)
@@ -168,28 +186,16 @@
                 step_summary = self.test_step(x_test, y_test)
 
                 # implement progress bar
                 if progress_bar is not None:
                     progress_bar.set_postfix(step_summary)
                     progress_bar.update()
 
-            # summarize
-            for name, fn in self.metric_fns.items():
-                if name.startswith("val_"):
-                    name = name.replace("val_", "")
-                try:
-                    summary[name] = float(fn.result.detach())
-                except Exception as metric_error:
-                    runtime_error = errors.MetricError(name)
-                    raise runtime_error from metric_error
-            if self.loss_fn is not None:
-                summary["loss"] = float(self.loss_fn.result.detach())
-
             # reset model and loss
-            return summary
+            return self.summary
         except KeyboardInterrupt:
             view.logger.info("Testing interrupted.")
             return {}
         except Exception as error:
             view.logger.error(error)
             runtime_error = errors.TestingError()
             raise runtime_error from error
@@ -209,35 +215,30 @@
         A single testing step
 
         - Parameters:
             - x_train: The testing data in `torch.Tensor`
             - y_train: The testing label in `torch.Tensor`
         - Returns: A `dict` of validation summary
         """
-        # initialize
-        summary: Dict[str, float] = {}
-
         # forward pass
         y = self.forward(x_test)
 
         # forward metrics
         for name, fn in self.compiled_metrics.items():
             if name.startswith("val_"):
                 name = name.replace("val_", "")
             elif "loss" in name:
                 continue
             try:
                 fn(y, y_test)
-                summary[name] = float(fn.result.detach())
             except Exception as metric_error:
                 runtime_error = errors.MetricError(name)
                 raise runtime_error from metric_error
 
         # forward loss
         if self.loss_fn is not None:
             try:
                 self.loss_fn(y, y_test)
-                summary["loss"] = float(self.loss_fn.result.detach())
             except Exception as loss_error:
                 runtime_error = errors.LossError()
                 raise loss_error from runtime_error
-        return summary
+        return self.summary
```

### Comparing `torchmanager_nightly-1.2b5/torchmanager/train/checkpoint.py` & `torchmanager_nightly-1.2b6/torchmanager/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/train/learning_rate.py` & `torchmanager_nightly-1.2b6/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager/training.py` & `torchmanager_nightly-1.2b6/torchmanager/training.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,15 +137,17 @@
     def backward(self, loss: torch.Tensor) -> None:
         """
         Backward function to calculate the gradients
         
         - Parameters:
             - loss: A `torch.Tensor` of loss value
         """
+        self.compiled_optimizer.zero_grad()
         loss.backward()
+        self.compiled_optimizer.step()
 
     def fit(self, training_dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, epochs: Optional[int] = None, val_dataset: Optional[Union[DataLoader[Any], Dataset[Any], Collection]] = None, callbacks_list: List[Callback] = [], *, iterations: Optional[int] = None, initial_epoch: Optional[int] = None, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, **kwargs) -> Module:
         """
         Training algorithm
 
         - Parameters:
             - training_dataset: Any kind of training dataset in `torch.utils.data.DataLoader` or `.data.Dataset`
@@ -266,40 +268,23 @@
 
         - Parameters:
             - x_train: The training data
             - y_train: The training label
         - Returns: A summary of `dict` with keys as `str` and values as `float`
         """
         # forward pass
-        summary: Dict[str, float] = {}
         y = self.forward(x_train)
         loss = self.compiled_losses(y, y_train)
 
+        # backward pass
+        self.backward(loss)
+
         # forward metrics
         for name, fn in self.compiled_metrics.items():
             if not name.startswith("val_") and "loss" not in name:
                 fn(y, y_train)
-
-        # backward pass
-        self.compiled_optimizer.zero_grad()
-        self.backward(loss)
-        self.compiled_optimizer.step()
-
-        # summary result
-        try:
-            summary["loss"] = float(self.compiled_losses.result.detach())
-        except Exception as e:
-            raise errors.LossError() from e
-        for name, fn in self.metric_fns.items():
-            if name.startswith("val_"):
-                continue
-            try:
-                summary[name] = float(fn.result.detach())
-            except Exception as metric_error:
-                runtime_error = errors.MetricError(name)
-                raise runtime_error from metric_error
-        return summary
+        return self.summary
 
     def to_checkpoint(self) -> Checkpoint[Self]:
         ckpt = super().to_checkpoint()
         ckpt.last_epoch = self.current_epoch
         return ckpt
```

### Comparing `torchmanager_nightly-1.2b5/torchmanager_core/devices/device.py` & `torchmanager_nightly-1.2b6/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager_core/errors/train.py` & `torchmanager_nightly-1.2b6/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager_core/protocols.py` & `torchmanager_nightly-1.2b6/torchmanager_core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager_core/random/seed.py` & `torchmanager_nightly-1.2b6/torchmanager_core/random/seed.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b5/torchmanager_core/version.py` & `torchmanager_nightly-1.2b6/torchmanager_core/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,31 +88,35 @@
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.2")
-CURRENT = Version("v1.2b5")
-DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 5)"
+CURRENT = Version("v1.2b6")
+DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 6)"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
 
 
-def deprecated(target_version: str, removing_version: str):
+def deprecated(target_version: Any, removing_version: Any):
     '''
     Deprecated decorator function
 
     - Parameters:
-        - target_version: A `str` of version for the deprecation
-        - removing_version: A `str` of version for removing
+        - target_version: `Any` type of version for the deprecation
+        - removing_version: `Any` type of version for removing
     '''
+    # format versions
+    target_version = Version(target_version)
+    removing_version = Version(removing_version)
+
     # define wrapping function
     def wrapping_fn(fn):
         @functools.wraps(fn)
         def deprecated_fn(*args, **kwargs):
             if CURRENT >= removing_version:
                 raise VersionError(fn.__name__, removing_version)
             elif CURRENT >= target_version:
```

### Comparing `torchmanager_nightly-1.2b5/PKG-INFO` & `torchmanager_nightly-1.2b6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2b5
-Summary: PyTorch Training Manager v1.2 (Beta 5)
+Version: 1.2b6
+Summary: PyTorch Training Manager v1.2 (Beta 6)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


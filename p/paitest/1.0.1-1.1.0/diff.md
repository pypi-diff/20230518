# Comparing `tmp/paitest-1.0.1-py3-none-any.whl.zip` & `tmp/paitest-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 25031 bytes, number of entries: 13
--rw-r--r--  2.0 unx       40 b- defN 80-Jan-01 00:00 paitest/__init__.py
+Zip file size: 25069 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 paitest/__init__.py
 -rw-r--r--  2.0 unx      342 b- defN 80-Jan-01 00:00 paitest/frames/__init__.py
 -rw-r--r--  2.0 unx     2581 b- defN 80-Jan-01 00:00 paitest/frames/coord.py
 -rw-r--r--  2.0 unx      823 b- defN 80-Jan-01 00:00 paitest/frames/coord.pyi
--rw-r--r--  2.0 unx    14448 b- defN 80-Jan-01 00:00 paitest/frames/frame.py
+-rw-r--r--  2.0 unx    14257 b- defN 80-Jan-01 00:00 paitest/frames/frame.py
 -rw-r--r--  2.0 unx     4707 b- defN 80-Jan-01 00:00 paitest/frames/frame_params.py
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 paitest/log.py
--rw-r--r--  2.0 unx    19934 b- defN 80-Jan-01 00:00 paitest/paitest.py
--rw-r--r--  2.0 unx     1786 b- defN 80-Jan-01 00:00 paitest/paitest.pyi
--rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 paitest-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3665 b- defN 80-Jan-01 00:00 paitest-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-1.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1001 b- defN 16-Jan-01 00:00 paitest-1.0.1.dist-info/RECORD
-13 files, 84168 bytes uncompressed, 23385 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx    18940 b- defN 80-Jan-01 00:00 paitest/paitest.py
+-rw-r--r--  2.0 unx     1990 b- defN 80-Jan-01 00:00 paitest/paitest.pyi
+-rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 paitest-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3763 b- defN 80-Jan-01 00:00 paitest-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 paitest-1.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1001 b- defN 16-Jan-01 00:00 paitest-1.1.0.dist-info/RECORD
+13 files, 83308 bytes uncompressed, 23423 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: paitest/paitest.py
 Comment: 
 
 Filename: paitest/paitest.pyi
 Comment: 
 
-Filename: paitest-1.0.1.dist-info/LICENSE
+Filename: paitest-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: paitest-1.0.1.dist-info/METADATA
+Filename: paitest-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: paitest-1.0.1.dist-info/WHEEL
+Filename: paitest-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: paitest-1.0.1.dist-info/RECORD
+Filename: paitest-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## paitest/__init__.py

```diff
@@ -1 +1,3 @@
 from .paitest import paitest as paitest
+
+__all__ = ["paitest"]
```

## paitest/frames/frame.py

```diff
@@ -112,19 +112,17 @@
 
         param_reg: List[int] = []
 
         if is_random:
             if not is_legal:
                 # Don't care 'tick_wait_start' split in #1 and #2
                 for _ in range(2):
-                    param_reg.append(random.randint(
-                        0, FM.GENERAL_PAYLOAD_MASK))
+                    param_reg.append(random.randint(0, FM.GENERAL_PAYLOAD_MASK))
 
-                param_reg[1] = (param_reg[1] & (
-                    ~CFM.TEST_CHIP_ADDR_HIGH3_MASK)) | high3
+                param_reg[1] = (param_reg[1] & (~CFM.TEST_CHIP_ADDR_HIGH3_MASK)) | high3
                 param_reg.append(low7 << CFM.TEST_CHIP_ADDR_LOW7_OFFSET)
             else:
                 # Do legal geenration
                 pass
         else:
             pass
 
@@ -343,49 +341,40 @@
 
     def _general_info(self) -> None:
         print("General info of frame: 0x%x" % self._frame)
         print("#1  Frame type:         %s" % self._get_subtype())
 
         chip_coord = self._get_chip_coord()
         print(
-            "#2  Chip coordinate:    [0x%02x | 0x%02x]" % (
-                chip_coord.x, chip_coord.y)
+            "#2  Chip coordinate:    [0x%02x | 0x%02x]" % (chip_coord.x, chip_coord.y)
         )
 
         core_coord = self._get_core_coord()
         print(
-            "#3  Core coordinate:    [0x%02x | 0x%02x]" % (
-                core_coord.x, core_coord.y)
+            "#3  Core coordinate:    [0x%02x | 0x%02x]" % (core_coord.x, core_coord.y)
         )
 
         core_star_coord = self._get_core_star_coord()
         print(
             "#4  Core* coordinate:   [0x%02x | 0x%02x]"
             % (core_star_coord.x, core_star_coord.y)
         )
 
     def _config2_info(self) -> None:
         print("Info of parameter registers")
-        print("#1  Weight width:       0x%x" %
-              self._param_reg_dict["weight_width"])
+        print("#1  Weight width:       0x%x" % self._param_reg_dict["weight_width"])
         print("#2  LCN:                0x%x" % self._param_reg_dict["LCN"])
-        print("#3  Input width:        0x%x" %
-              self._param_reg_dict["input_width"])
-        print("#4  Spike width:        0x%x" %
-              self._param_reg_dict["spike_width"])
-        print("#5  Neuron num:         %d" %
-              self._param_reg_dict["neuron_num"])
+        print("#3  Input width:        0x%x" % self._param_reg_dict["input_width"])
+        print("#4  Spike width:        0x%x" % self._param_reg_dict["spike_width"])
+        print("#5  Neuron num:         %d" % self._param_reg_dict["neuron_num"])
         print("#6  Pool max enable:    %d" % self._param_reg_dict["pool_max"])
-        print("#7  Tick wait start:    0x%x" %
-              self._param_reg_dict["tick_wait_start"])
-        print("#8  Tick wait end:      0x%x" %
-              self._param_reg_dict["tick_wait_end"])
+        print("#7  Tick wait start:    0x%x" % self._param_reg_dict["tick_wait_start"])
+        print("#8  Tick wait end:      0x%x" % self._param_reg_dict["tick_wait_end"])
         print("#9  SNN enable:         %d" % self._param_reg_dict["SNN_EN"])
-        print("#10 Target LCN:         0x%x" %
-              self._param_reg_dict["target_LCN"])
+        print("#10 Target LCN:         0x%x" % self._param_reg_dict["target_LCN"])
 
         # type: ignore
         test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"]
         print(
             "#11 Test chip coord:    [0x%02x | 0x%02x]"
             % (test_chip_coord.x, test_chip_coord.y)
         )
@@ -431,16 +420,15 @@
         ) & CFM.SNN_EN_MASK
         self._param_reg_dict["target_LCN"] = (
             self._frames_group[1] >> CFM.TARGET_LCN_OFFSET
         ) & CFM.TARGET_LCN_MASK
 
         high3 = self._frames_group[1] >> CFM.TEST_CHIP_ADDR_HIGH3_OFFSET
         low7 = self._frames_group[2] >> CFM.TEST_CHIP_ADDR_LOW7_OFFSET
-        self._param_reg_dict["test_chip_coord"] = test_chip_addr_combine(
-            high3, low7)
+        self._param_reg_dict["test_chip_coord"] = test_chip_addr_combine(high3, low7)
 
     def _decode_direction(self) -> Direction:
         # type: ignore
         test_chip_coord: Coord = self._param_reg_dict["test_chip_coord"]
         offset = test_chip_coord - self._get_chip_coord()
 
         try:
```

## paitest/paitest.py

```diff
@@ -8,26 +8,24 @@
 from .frames import FrameSubType as FST
 from .log import logger
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 
 
-__all__ = ["paitest"]
-
-
 class paitest:
     def __init__(
         self,
         direction="EAST",
         fixed_chip_coord: Tuple[int, int] = (0, 0),
     ) -> None:
         """
-        :param direction: The direction relative to the PAICORE. Default is 'EAST'.
-        :param fixed_chip_coord: The chip address of the PAICORE under test. Default is (0, 0).
+        Params:
+        - direction: The direction relative to the PAICORE. Default is 'EAST'.
+        - fixed_chip_coord: The chip address of the PAICORE under test. Default is (0, 0).
         """
         self._verbose: bool = True
         self._fixed_chip_coord: Coord = Coord(fixed_chip_coord)
         self._masked_core_coord: Coord
         self._fixed_core_star_coord: Coord = Coord(0, 0)
         self._test_chip_coord: Coord
 
@@ -35,20 +33,20 @@
 
     def Get1GroupForNCoresWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
-        gen_txt: bool = False,
         verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
         """
         Generate 1 group(case) for 'N' random cores coordinates with 'N' different parameters.
 
+        Params:
         - `N`: How many cores coordinates under test.
         - `save_dir`: Where to save the frames files.
         - `masked_core_coord`: to avoid generating the specific core coordinate.
         - `gen_txt`: to save frames into text files instead of default binary files.
         - `verbose`: whether to display the log.
 
         :return: 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
@@ -115,34 +113,28 @@
 
             if verbose:
                 logger.info(
                     "Test in frame  #1/1:  0x%x in group #%d/%d"
                     % (testin_frame, i + 1, N)
                 )
 
-        if isinstance(work_dir, Path):
-            _suffix = ".txt" if gen_txt else ".bin"
-            self.SaveFrames(work_dir / ("config" + _suffix), cf_list, verbose)
-            self.SaveFrames(work_dir / ("testin" + _suffix), ti_list, verbose)
-            self.SaveFrames(work_dir / ("testout" + _suffix), to_list, verbose)
-
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def Get1GroupForNCoresWith1Param(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
-        gen_txt: bool = False,
         verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
         """
         Generate 1 group(case) for 'N' random cores coordinates with the same parameters.
 
+        Params:
         - `N`: How many cores coordinates under test.
         - `save_dir`: Where to save the frames files.
         - `masked_core_coord`: to avoid generating the specific core coordinate.
         - `gen_txt`: to save frames into text files instead of default binary files.
         - `verbose`: whether to display the log.
 
         :return: 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
@@ -208,34 +200,28 @@
 
             if verbose:
                 logger.info(
                     "Test in frame  #1/1:  0x%x in group #%d/%d"
                     % (testin_frame, i + 1, N)
                 )
 
-        if isinstance(work_dir, Path):
-            _suffix = ".txt" if gen_txt else ".bin"
-            self.SaveFrames(work_dir / ("config" + _suffix), cf_list, verbose)
-            self.SaveFrames(work_dir / ("testin" + _suffix), ti_list, verbose)
-            self.SaveFrames(work_dir / ("testout" + _suffix), to_list, verbose)
-
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def GetNGroupsFor1CoreWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
-        gen_txt: bool = False,
         verbose: bool = False,
     ) -> Tuple[Tuple[int, ...], ...]:
         """
         Generate 'N' groups(cases) for 1 random core coordinate with 'N' different parameters.
 
+        Params:
         - `N`: How many test groups(cases) of 1 core will be generated.
         - `save_dir`: Where to save the frames files.
         - `masked_core_coord`: to avoid generating the specific core coordinate.
         - `gen_txt`: to save frames into text files instead of default binary files.
         - `verbose`: whether to display the log.
 
         :return: 3 tuples including config, testin & testout tuples. 3*N frames in config & testout tuple and N frames in testin tuple.
@@ -301,32 +287,29 @@
 
             if verbose:
                 logger.info(
                     "Test in frame  #1/1:  0x%x in group #%d/%d"
                     % (testin_frame, i + 1, N)
                 )
 
-        if isinstance(work_dir, Path):
-            _suffix = ".txt" if gen_txt else ".bin"
-            self.SaveFrames(work_dir / ("config" + _suffix), cf_list, verbose)
-            self.SaveFrames(work_dir / ("testin" + _suffix), ti_list, verbose)
-            self.SaveFrames(work_dir / ("testout" + _suffix), to_list, verbose)
-
         return tuple(cf_list), tuple(ti_list), tuple(to_list)
 
     def ReplaceCoreCoord(
         self,
         frames: Union[int, List[int], Tuple[int, ...]],
         new_core_coord: Optional[Union[Tuple[int, int], Coord]] = None,
     ) -> Union[int, Tuple[int, ...]]:
         """
         Replace the core coordinate with the new one.
 
+        Params:
         - frames: of which the core coordinate you want to replace. It can be a single frame, or a list or tuple.
         - new_core_coord: The new core coordinate. If not specified, it will generate one randomly.
+
+        :return: the frame or frames after replacement.
         """
         if isinstance(frames, int):
             _frame = frames
         else:
             _frame = frames[0]
 
         if isinstance(new_core_coord, Tuple):
@@ -349,53 +332,59 @@
             _frames = list(frames)
             return self._ReplaceCoreCoordInNFrames(_frames, _new_core_coord)
 
     @staticmethod
     def SaveFrames(
         save_path: Union[str, Path],
         frames: Union[int, List[int], Tuple[int, ...]],
-        verbose: bool = False,
+        byteorder="big",
     ) -> None:
         """
-        Write frames into specific binary file. Files with '.bin' suffix is recommended
+        Write frames into specific text or binary file. Files with '.bin' suffix is recommended.
 
-        Support .txt files as well.
-
-        - gen_txt: Wether to generate txt files.
+        Params:
+        - save_path: The path of files.
+        - frames: A single frame or list or tuple of frames.
+        - byteorder: Big or little-edian format.
         """
 
         _path = Path(save_path)
         _suffix: str = _path.suffix
 
         if _suffix != ".bin" and _suffix != ".txt":
-            raise NotImplementedError(
-                f"File with suffix {_suffix} is not supported!")
+            raise NotImplementedError(f"File with suffix {_suffix} is not supported!")
+
+        assert byteorder in ["little", "big"]
 
         if _suffix == ".bin":
             with open(_path, "wb") as f:
                 if isinstance(frames, int):
-                    f.write(frames.to_bytes(8, "big"))
+                    f.write(frames.to_bytes(8, byteorder))
                 else:
                     for frame in frames:
-                        f.write(frame.to_bytes(8, "big"))
+                        f.write(frame.to_bytes(8, byteorder))
 
         else:
+            if byteorder == "little":
+                logger.warning(
+                    "Saving into txt file in little-edian format is not supported!"
+                )
+
             with open(_path, "w") as f:  # Open with "w"
                 if isinstance(frames, int):
                     _str64 = bin(frames).split("0b")[1]
                     _str64 = _str64.zfill(64)
                     f.write(_str64 + "\n")
                 else:
                     for frame in frames:
                         _str64 = bin(frame).split("0b")[1]
                         _str64 = _str64.zfill(64)
                         f.write(_str64 + "\n")
 
-        if verbose:
-            logger.info(f"Saved frame(s) into {_path} OK")
+        logger.info(f"Saved frame(s) into {_path} OK")
 
     def _Get1CoreCoord(self, masked_coord: Optional[Coord] = None) -> Coord:
         """
         Generate a random core coordinate. Indicate the masked one to avoid generating the same one
         """
         return self._GetNCoresCoord(N=1, masked_coord=masked_coord)[0]
 
@@ -442,14 +431,16 @@
         self,
         N: int,
         core_coords: Union[List[Coord], Coord],
         is_legal: bool = False,
     ) -> List[Tuple[int, ...]]:
         """
         Generate 'N' random parameters register.
+
+        Params:
         - `is_legal`: whether to generate legal parameters for every core
         """
 
         def _ParamGenerator():
             test_chip_coord: Coord = self._direction.value + self._fixed_chip_coord
 
             while True:
@@ -499,56 +490,44 @@
         mask = FM.GENERAL_MASK & (
             ~(FM.GENERAL_CORE_ADDR_MASK << FM.GENERAL_CORE_ADDR_OFFSET)
         )
 
         new_core_addr = Coord2Addr(new_core_coord)
 
         for i, frame in enumerate(frames):
-            frames[i] = (frame & mask) | (
-                new_core_addr << FM.GENERAL_CORE_ADDR_OFFSET)
+            frames[i] = (frame & mask) | (new_core_addr << FM.GENERAL_CORE_ADDR_OFFSET)
 
         return tuple(frames)
 
     def _ReplaceHeader(self, frame: int, header: FST) -> int:
         """Replace the header of a frame with the new one."""
-        mask = FM.GENERAL_MASK & (
-            ~(FM.GENERAL_HEADER_MASK << FM.GENERAL_HEADER_OFFSET))
+        mask = FM.GENERAL_MASK & (~(FM.GENERAL_HEADER_MASK << FM.GENERAL_HEADER_OFFSET))
 
         return (frame & mask) | (header.value << FM.GENERAL_HEADER_OFFSET)
 
     def _ensure_dir(self, user_dir: Union[str, Path]) -> Path:
         _user_dir: Path = Path(user_dir)
 
         if not _user_dir.exists():
             logger.warning(f"Creating directory {_user_dir}...")
             _user_dir.mkdir(parents=True, exist_ok=True)
 
         return _user_dir
 
     def _ensure_cores(self, Ncores: int) -> None:
+        """Parameter check: Ncores"""
         if Ncores > 1024 - 16 or Ncores < 1:
             raise ValueError("Range of Ncores is 0 < N < 1008")
 
-    if sys.version_info >= (3, 8):
-
-        def _ensure_direction(
-            self, direction: Literal["EAST", "SOUTH", "WEST", "NORTH"]
-        ) -> None:
-            try:
-                self._direction = Direction[direction.upper()]
-            except KeyError:
-                raise KeyError(f"{direction} is an illegal direction!")
-
-    else:
-
-        def _ensure_direction(self, direction: str) -> None:
-            try:
-                self._direction = Direction[direction.upper()]
-            except KeyError:
-                raise KeyError(f"{direction} is an illegal direction!")
+    def _ensure_direction(self, direction: str) -> None:
+        """Parameter check: direction"""
+        try:
+            self._direction = Direction[direction.upper()]
+        except KeyError:
+            raise KeyError(f"{direction} is an illegal direction!")
 
     def _ensure_coord(self, coord: Coord) -> None:
+        """Parameter check: coord"""
         if coord >= Coord(0b11100, 0b11100):
-            raise ValueError(
-                "Address coordinate must: 0 <= x < 28 or 0 <= y < 28")
+            raise ValueError("Address coordinate must: 0 <= x < 28 or 0 <= y < 28")
 
         self._masked_core_coord = coord
```

## paitest/paitest.pyi

```diff
@@ -1,15 +1,14 @@
 import sys
+from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 
-from pathlib import Path
-
 class paitest:
     if sys.version_info >= (3, 8):
         def __init__(
             self,
             direction: Literal["EAST", "SOUTH", "WEST", "NORTH"] = "EAST",
             fixed_chip_coord: Tuple[int, int] = (0, 0),
         ) -> None: ...
@@ -22,39 +21,45 @@
 
     def Get1GroupForNCoresWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
-        gen_txt: bool = False,
         verbose: bool = False
     ) -> Tuple[Tuple[int, ...], ...]: ...
     def Get1GroupForNCoresWith1Param(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
-        gen_txt: bool = False,
         verbose: bool = False
     ) -> Tuple[Tuple[int, ...], ...]: ...
     def GetNGroupsFor1CoreWithNParams(
         self,
         N: int,
         *,
         save_dir: Optional[Union[str, Path]] = None,
         masked_core_coord: Optional[Tuple[int, int]] = None,
-        gen_txt: bool = False,
         verbose: bool = False
     ) -> Tuple[Tuple[int, ...], ...]: ...
     def ReplaceCoreCoord(
         self,
         frames: Union[int, List[int], Tuple[int, ...]],
         new_core_coord: Tuple[int, int],
     ) -> int: ...
-    @staticmethod
-    def SaveFrames(
-        save_path: Union[str, Path],
-        frames: Union[int, List[int], Tuple[int, ...]],
-        verbose: bool = False,
-    ) -> None: ...
+
+    if sys.version_info >= (3, 8):
+        @staticmethod
+        def SaveFrames(
+            save_path: Union[str, Path],
+            frames: Union[int, List[int], Tuple[int, ...]],
+            byteorder: Literal["little", "big"] = "big",
+        ) -> None: ...
+    else:
+        @staticmethod
+        def SaveFrames(
+            save_path: Union[str, Path],
+            frames: Union[int, List[int], Tuple[int, ...]],
+            byteorder: str = "big",
+        ) -> None: ...
```

## Comparing `paitest-1.0.1.dist-info/LICENSE` & `paitest-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `paitest-1.0.1.dist-info/METADATA` & `paitest-1.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paitest
-Version: 1.0.1
+Version: 1.1.0
 Summary: Test module for PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAITest
 License: AGPL v3.0
 Keywords: PAICookers,PAITest,PAICORE
 Author: KafCoppelia
 Author-email: k740677208@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -24,17 +24,17 @@
 
 # PAITest
 
 </div>
 
 ## 📦 版本
 
-[v1.0.1](https://github.com/PAICookers/PAITest/releases/tag/v1.0.1)
+[v1.1.0](https://github.com/PAICookers/PAITest/releases/tag/v1.1.0)
 
-✨支持 `.txt` 格式输出
+✨支持大/小端格式输出
 
 ## 🛠️ 使用生成
 
 配置帧及对应测试输入帧，以实现硬件通路的简单测试，后续将芯片实际测试输出帧与预期结果进行对比即可。
 
 ⚠️ 由于配置帧/测试帧I型需要配合串口配置使用，因此目前仅采用**配置/测试帧II型**方案，且 `CHIP_ADDR` 与 `CORE*_ADDR` 均固定为 `(0, 0)`。
 
@@ -57,15 +57,15 @@
    cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups, save_dir=save_to_dir, verbose=True)
 
    # Mask a cord coordinate so that avoid generating the same coordinate.
    cf, ti, to = PAITestManager.Get1GroupForNCoresWithNParams(groups,
        save_dir=save_to_dir, masked_core_coord=(12, 16), gen_txt=True)
    ```
 
-   ⚠️ 指定 `verbose=True` 以开启日志显示，默认关闭；指定 `gen_txt=True` 以保存至 `.txt`，默认保存至 `.bin`。
+   ⚠️ 指定 `verbose=True` 以开启日志显示，默认关闭
 
 3. `Get1GroupForNCoresWith1Param`，产生1组针对 `N` 个核的配置-测试帧，每个核配置**相同参数**。可以指定单个需要**屏蔽**的核坐标
 
    ```python
    # Same as Get1GroupForNCoresWithNParams
    cf, ti, to = PAITestManager.Get1GroupForNCoresWith1Param(10, save_dir="./test")
    ```
@@ -82,23 +82,25 @@
    ```python
    # Replaced core coordinate with (9, 9)
    replaced = PAITestManager.ReplaceCoreCoord(original_frames, (9, 9))
    ```
 
    ⚠️ 一组指一组完整的配置帧，包含3帧。对于测试输入帧，即为单帧。
 
-6. `SaveFrames`，默认保存帧数据至指定文件，支持 `.bin` 或 `.txt` 格式
+6. `SaveFrames`，保存帧数据至指定文件，支持 `.bin` 或 `.txt` 格式，支持指定大/小端输出
 
    ```python
-   # Save into binary files
-   PAITestManager.SaveFrames("./test/config.bin", replaced)
+   # Save into binary files with big-edian format(default)
+   PAITestManager.SaveFrames("./test/config.bin", replaced, byteorder="big")
 
    # Or text files
    PAITestManager.SaveFrames("./test/config.txt", replaced)
    ```
 
+   ⚠️ 指定 `byteorder="big"/"little"` 以大/小端格式储存帧数据，默认大端
+
 ## 🗓️ TODO
 
 - [x] 上板验证
 - [ ] 参数检验
 - [ ] 配置/测试帧III/IV型
```


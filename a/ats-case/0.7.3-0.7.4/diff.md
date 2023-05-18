# Comparing `tmp/ats_case-0.7.3.tar.gz` & `tmp/ats_case-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.7.3.tar", last modified: Fri May 12 07:45:03 2023, max compression
+gzip compressed data, was "ats_case-0.7.4.tar", last modified: Thu May 18 05:26:22 2023, max compression
```

## Comparing `ats_case-0.7.3.tar` & `ats_case-0.7.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 07:45:03.661284 ats_case-0.7.3/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.7.3/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-05-12 07:45:03.658298 ats_case-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 07:45:03.278310 ats_case-0.7.3/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.7.3/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:45:03.480767 ats_case-0.7.3/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.7.3/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17714 2023-05-12 07:44:28.000000 ats_case-0.7.3/ats_case/case/command.py
--rw-rw-rw-   0        0        0    10440 2023-05-12 07:33:23.000000 ats_case-0.7.3/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.7.3/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5548 2023-05-04 06:36:02.000000 ats_case-0.7.3/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:45:03.541603 ats_case-0.7.3/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.7.3/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.7.3/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.7.3/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:45:03.596456 ats_case-0.7.3/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.3/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.7.3/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.7.3/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:45:03.638344 ats_case-0.7.3/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.3/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.7.3/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-05-12 07:45:03.374051 ats_case-0.7.3/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-05-12 07:45:01.000000 ats_case-0.7.3/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-05-12 07:45:02.000000 ats_case-0.7.3/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 07:45:01.000000 ats_case-0.7.3/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-12 07:45:02.000000 ats_case-0.7.3/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 07:45:02.000000 ats_case-0.7.3/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 07:45:03.661284 ats_case-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-05-12 07:44:28.000000 ats_case-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.703630 ats_case-0.7.4/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.7.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-05-18 05:26:22.701635 ats_case-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.231452 ats_case-0.7.4/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.7.4/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.519102 ats_case-0.7.4/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.7.4/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17907 2023-05-18 03:07:32.000000 ats_case-0.7.4/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    11101 2023-05-18 05:15:05.000000 ats_case-0.7.4/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.7.4/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5548 2023-05-04 06:36:02.000000 ats_case-0.7.4/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.590910 ats_case-0.7.4/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.7.4/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.7.4/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.7.4/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.655738 ats_case-0.7.4/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.4/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.7.4/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.7.4/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.693654 ats_case-0.7.4/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.4/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2473 2023-05-18 05:24:57.000000 ats_case-0.7.4/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-05-18 05:26:22.368106 ats_case-0.7.4/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 05:26:21.000000 ats_case-0.7.4/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 05:26:22.704628 ats_case-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-05-17 05:57:29.000000 ats_case-0.7.4/setup.py
```

### Comparing `ats_case-0.7.3/PKG-INFO` & `ats_case-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.7.3
+Version: 0.7.4
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.7.3/README.md` & `ats_case-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.3/ats_case/case/command.py` & `ats_case-0.7.4/ats_case/case/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     :param param: desc-测试步骤描述
     :return:
     """
     desc = param.get('desc')
 
     def decorate(callback):
         def fn(*args, **kwargs):
-            client().message({'msg': desc}).show(args[0])  # send(args[0], todo={'app:show': {'msg': desc}})
+            client().message(desc).show(args[0])  # send(args[0], todo={'app:show': {'msg': desc}})
             r = callback(*args, **kwargs)
             return r
 
         return fn
 
     return decorate
 
@@ -284,14 +284,16 @@
 
             logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
                 self._func_module, self._func, self._func_parameter))
             result = udm.handle(module='meter.{}'.format(self._func_module), function=self._func
                                 , data=data, debug_url=context.acd_url)
             logger.info('~ @ACD<- module:{} function:{} result:{}'.format(self._func_module, self._func, result))
 
+            context.runtime.acvs[context.runtime.step] = result
+
         return result
 
     def exec(self, context: Context):
         self.encode(context)
         result = send(context,
                       todo={'meter:comm': {'channel': context.case.steps[str(context.runtime.step)].get('channel'),
                                            'frame': self._frame}})
@@ -350,14 +352,16 @@
 
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             self._protocol.name, self._operation, self._parameter))
         result = udm.handle(module='em.{}'.format(self._protocol.name), function=self._operation
                             , data=data, debug_url=context.acd_url)
         logger.info('~ @ACD<- module:{} function:{} result:{}'.format(self._protocol.name, self._operation, result))
 
+        context.runtime.acvs[context.runtime.step] = result
+
         return result
 
     def exec(self, context: Context):
         self.handle(context)
         send(context, todo={'app:show': {'msg': self.acv(context)}})
 
 
@@ -432,14 +436,16 @@
 
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             'bench', self._operation, self._result))
         result = udm.handle(module='bench', function=self._operation
                             , data=data, debug_url=context.acd_url)
         logger.info('~ @ACD<- module:{} function:{} result:{}'.format('bench', self._operation, result))
 
+        context.runtime.acvs[context.runtime.step] = result
+
         return result
 
     def _flush(self, context: Context):
         context.runtime.steps.update({context.runtime.step: func.to_dict(obj='bench', op=self._operation
                                                                          , parameter=self._parameter,
                                                                          result=self._result)})
 
@@ -484,15 +490,15 @@
         self._parameter = None
 
     def operation(self, command: str):
         self._operation = command
         return self
 
     def message(self, msg):
-        self._message = msg
+        self._message = {'msg': msg}
         return self
 
     def parameter(self, param=None):
         self._parameter = param
         return self
 
     def show(self, context: Context, types=2):
```

### Comparing `ats_case-0.7.3/ats_case/case/context.py` & `ats_case-0.7.4/ats_case/case/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -306,14 +306,28 @@
             self._loop_start_step = 0
             self._loop_end_step = 0
             self._loop_count = 0
             self._loop_index = 0
             self._steps = {}
             # 多帧时使用
             self._final_result = None
+            # 对比结果 - 用例结束时统计执行结果
+            self._acvs = {}
+
+        def acv_result(self):
+            sc = fc = 0
+            fs = []
+            for s, result in self.acvs.items():
+                if str(result).find('合格') >= 0:
+                    sc += 1
+                else:
+                    fc += 1
+                    fs.append(s)
+
+            return '{} 步, {} 合格, {} 不合格 - {}'.format(len(self._acvs), sc, fc, ','.join(fs))
 
         @property
         def step(self):
             return self._step
 
         @step.setter
         def step(self, value):
@@ -367,14 +381,22 @@
         def final_result(self):
             return self._final_result
 
         @final_result.setter
         def final_result(self, value):
             self._final_result = value
 
+        @property
+        def acvs(self):
+            return self._acvs
+
+        @acvs.setter
+        def acvs(self, value):
+            self._acvs = value
+
     class Session(object):
         def __init__(self, parent):
             self._parent = parent
 
         def get(self, name: str, key: str):
             return mm.Dict.get('{}:{}'.format(self._parent.test_sn, name), key)
```

### Comparing `ats_case-0.7.3/ats_case/case/executor.py` & `ats_case-0.7.4/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.3/ats_case/case/translator.py` & `ats_case-0.7.4/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.3/ats_case/common/error.py` & `ats_case-0.7.4/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.3/ats_case/manage/core.py` & `ats_case-0.7.4/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.3/ats_case/manage/start.py` & `ats_case-0.7.4/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.3/ats_case/template/testcase_v1.tmp` & `ats_case-0.7.4/ats_case/template/testcase_v1.tmp`

 * *Files 15% similar despite different names*

```diff
@@ -9,30 +9,34 @@
         测试用例前置步骤
         :return:
         """
         logger.info('~ @TCC-MSG-> TEST CASE[{}-{}] METER[{}] START...'.format(CaseContext.case.id,
                                                                               CaseContext.case.name,
                                                                               CaseContext.meter.no))
         try:
-            msg = {'msg': '[{}]开始测试 - 测试用例[{}], 电表[{}]...'.format(
-                                  func.sys_current_time(), CaseContext.case.name, CaseContext.meter.no)}
+            msg = '==============================================================================================\r\n'
+            msg += '[{}]开始测试 - 测试用例[{}], 电表[{}]...\r\n'.format(
+                                  func.sys_current_time(), CaseContext.case.name, CaseContext.meter.no)
             command.client().message(msg).show(CaseContext, types=0)
         except APIError as ae:
             logger.info(str(ae))
             raise AssertionError(str(ae))
 
     @pytest.mark.run(order=3)
     def test_after(self, CaseContext):
         """
         测试用例后置步骤
         :return:
         """
         try:
-            msg = {'msg': '[{}]结束测试 - 测试用例[{}], 电表[{}].'.format(
-                                  func.sys_current_time(), CaseContext.case.name, CaseContext.meter.no)}
+            msg = '[{}]结束测试 - 测试用例[{}], 电表[{}].\r\n'.format(func.sys_current_time(),
+                                                              CaseContext.case.name,
+                                                              CaseContext.meter.no)
+            msg += '----------------------------------------------------------------------------------------------\r\n'
+            msg += '测试结果: {}\r\n'.format(CaseContext.runtime.acv_result())
             command.client().message(msg).show(CaseContext, types=1)
         except APIError as ae:
             logger.info(str(ae))
             raise AssertionError(str(ae))
 
         logger.info('~ @TCC-MSG-> TEST CASE[{}-{}] METER[{}] END.'.format(CaseContext.case.id,
                                                                           CaseContext.case.name,
```

### Comparing `ats_case-0.7.3/ats_case.egg-info/PKG-INFO` & `ats_case-0.7.4/ats_case.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.7.3
+Version: 0.7.4
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.7.3/ats_case.egg-info/SOURCES.txt` & `ats_case-0.7.4/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.3/setup.py` & `ats_case-0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.7.3",
+    version="0.7.4",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```


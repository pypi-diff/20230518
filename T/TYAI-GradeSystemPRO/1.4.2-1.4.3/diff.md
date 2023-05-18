# Comparing `tmp/TYAI-GradeSystemPRO-1.4.2.tar.gz` & `tmp/TYAI-GradeSystemPRO-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TYAI-GradeSystemPRO-1.4.2.tar", last modified: Thu May 18 15:01:46 2023, max compression
+gzip compressed data, was "TYAI-GradeSystemPRO-1.4.3.tar", last modified: Thu May 18 15:29:08 2023, max compression
```

## Comparing `TYAI-GradeSystemPRO-1.4.2.tar` & `TYAI-GradeSystemPRO-1.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 15:01:46.765361 TYAI-GradeSystemPRO-1.4.2/
-drwxrwxrwx   0        0        0        0 2023-05-18 15:01:46.745025 TYAI-GradeSystemPRO-1.4.2/MainPackge/
--rw-rw-rw-   0        0        0     9811 2023-05-18 14:38:22.000000 TYAI-GradeSystemPRO-1.4.2/MainPackge/TYAIWebUpDate1.4.2.py
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:34.000000 TYAI-GradeSystemPRO-1.4.2/MainPackge/__init__.py
--rw-rw-rw-   0        0        0      152 2023-05-18 15:01:46.764865 TYAI-GradeSystemPRO-1.4.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 15:01:46.763873 TYAI-GradeSystemPRO-1.4.2/TYAI_GradeSystemPRO.egg-info/
--rw-rw-rw-   0        0        0      152 2023-05-18 15:01:46.000000 TYAI-GradeSystemPRO-1.4.2/TYAI_GradeSystemPRO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-18 15:01:46.000000 TYAI-GradeSystemPRO-1.4.2/TYAI_GradeSystemPRO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 15:01:46.000000 TYAI-GradeSystemPRO-1.4.2/TYAI_GradeSystemPRO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-18 15:01:46.000000 TYAI-GradeSystemPRO-1.4.2/TYAI_GradeSystemPRO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-18 15:01:46.000000 TYAI-GradeSystemPRO-1.4.2/TYAI_GradeSystemPRO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 15:01:46.765857 TYAI-GradeSystemPRO-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      537 2023-05-18 14:59:34.000000 TYAI-GradeSystemPRO-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:29:08.016146 TYAI-GradeSystemPRO-1.4.3/
+-rw-rw-rw-   0        0        0      152 2023-05-18 15:29:08.015649 TYAI-GradeSystemPRO-1.4.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 15:29:07.998786 TYAI-GradeSystemPRO-1.4.3/TYAI-GradeSystemPRO/
+-rw-rw-rw-   0        0        0     9811 2023-05-18 14:38:22.000000 TYAI-GradeSystemPRO-1.4.3/TYAI-GradeSystemPRO/TYAIWebUpDate1.4.2.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:34.000000 TYAI-GradeSystemPRO-1.4.3/TYAI-GradeSystemPRO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:29:08.014657 TYAI-GradeSystemPRO-1.4.3/TYAI_GradeSystemPRO.egg-info/
+-rw-rw-rw-   0        0        0      152 2023-05-18 15:29:07.000000 TYAI-GradeSystemPRO-1.4.3/TYAI_GradeSystemPRO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-18 15:29:07.000000 TYAI-GradeSystemPRO-1.4.3/TYAI_GradeSystemPRO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 15:29:07.000000 TYAI-GradeSystemPRO-1.4.3/TYAI_GradeSystemPRO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-18 15:29:07.000000 TYAI-GradeSystemPRO-1.4.3/TYAI_GradeSystemPRO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-18 15:29:07.000000 TYAI-GradeSystemPRO-1.4.3/TYAI_GradeSystemPRO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 15:29:08.016146 TYAI-GradeSystemPRO-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      546 2023-05-18 15:29:04.000000 TYAI-GradeSystemPRO-1.4.3/setup.py
```

### Comparing `TYAI-GradeSystemPRO-1.4.2/MainPackge/TYAIWebUpDate1.4.2.py` & `TYAI-GradeSystemPRO-1.4.3/TYAI-GradeSystemPRO/TYAIWebUpDate1.4.2.py`

 * *Files identical despite different names*

### Comparing `TYAI-GradeSystemPRO-1.4.2/setup.py` & `TYAI-GradeSystemPRO-1.4.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name='TYAI-GradeSystemPRO',  # 包名称
-    version='1.4.2',  # 版本号
+    version='1.4.3',  # 版本号
     description='TYAI Web Update Package',  # 包描述
     author='Yihuan',  # 作者姓名
     author_email='ivan17.lai@gmail.com',  # 作者电子邮件
-    packages=['MainPackge'],  # 包含的子包列表
+    packages=['TYAI-GradeSystemPRO'],  # 包含的子包列表
     install_requires=[  # 安装所需的依赖包列表
         'selenium',
         'beautifulsoup4',
         'keras',
         'opencv-python',
         'Pillow',
         'tensorflow'
```


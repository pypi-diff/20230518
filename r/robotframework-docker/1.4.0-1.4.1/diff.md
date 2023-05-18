# Comparing `tmp/robotframework-docker-1.4.0.tar.gz` & `tmp/robotframework-docker-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-docker-1.4.0.tar", last modified: Sun Nov 20 16:32:59 2022, max compression
+gzip compressed data, was "robotframework-docker-1.4.1.tar", last modified: Wed Nov 30 16:06:19 2022, max compression
```

## Comparing `robotframework-docker-1.4.0.tar` & `robotframework-docker-1.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 16:32:59.400711 robotframework-docker-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-20 16:32:48.000000 robotframework-docker-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-11-20 16:32:59.400711 robotframework-docker-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-11-20 16:32:48.000000 robotframework-docker-1.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-20 16:32:59.400711 robotframework-docker-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-11-20 16:32:48.000000 robotframework-docker-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 16:32:59.400711 robotframework-docker-1.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (121)    31581 2022-11-20 16:32:48.000000 robotframework-docker-1.4.0/src/DockerComposeLibrary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 16:32:59.400711 robotframework-docker-1.4.0/src/robotframework_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-11-20 16:32:59.000000 robotframework-docker-1.4.0/src/robotframework_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-20 16:32:59.000000 robotframework-docker-1.4.0/src/robotframework_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-20 16:32:59.000000 robotframework-docker-1.4.0/src/robotframework_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-20 16:32:59.000000 robotframework-docker-1.4.0/src/robotframework_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-20 16:32:59.000000 robotframework-docker-1.4.0/src/robotframework_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:06:19.436819 robotframework-docker-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-11-30 16:06:11.000000 robotframework-docker-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2022-11-30 16:06:19.436819 robotframework-docker-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2022-11-30 16:06:11.000000 robotframework-docker-1.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 16:06:19.436819 robotframework-docker-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2022-11-30 16:06:11.000000 robotframework-docker-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:06:19.436819 robotframework-docker-1.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    31715 2022-11-30 16:06:11.000000 robotframework-docker-1.4.1/src/DockerComposeLibrary.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:06:19.436819 robotframework-docker-1.4.1/src/robotframework_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2022-11-30 16:06:19.000000 robotframework-docker-1.4.1/src/robotframework_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2022-11-30 16:06:19.000000 robotframework-docker-1.4.1/src/robotframework_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 16:06:19.000000 robotframework-docker-1.4.1/src/robotframework_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2022-11-30 16:06:19.000000 robotframework-docker-1.4.1/src/robotframework_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2022-11-30 16:06:19.000000 robotframework-docker-1.4.1/src/robotframework_docker.egg-info/top_level.txt
```

### Comparing `robotframework-docker-1.4.0/LICENSE` & `robotframework-docker-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-docker-1.4.0/PKG-INFO` & `robotframework-docker-1.4.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: robotframework-docker
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Robot Framework Docker Library
 Home-page: https://github.com/vogoltsov/robotframework-docker
 Author: Vitaly Ogoltsov
 Author-email: vitaly.ogoltsov@me.com
 License: Apache License 2.0
 Keywords: testing testautomation robotframework docker docker-compose
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Robot Framework :: Library
 License-File: LICENSE
 
 Short Description
 -----------------
 
 `Robot Framework`_ library for working with ``docker`` and
```

### Comparing `robotframework-docker-1.4.0/README.rst` & `robotframework-docker-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-docker-1.4.0/setup.py` & `robotframework-docker-1.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,34 @@
 
 # Get the long description from the README file
 with open(os.path.join(here, 'README.rst'), encoding='utf-8') as readme_file:
     long_description = readme_file.read().split('long_description split')[1].strip()
 
 setup(
     name='robotframework-docker',
-    version='1.4.0',
+    version='1.4.1',
     description='A Robot Framework Docker Library',
     long_description=long_description,
     url='https://github.com/vogoltsov/robotframework-docker',
     author='Vitaly Ogoltsov',
     author_email='vitaly.ogoltsov@me.com',
     license='Apache License 2.0',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Testing',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Robot Framework :: Library',
     ],
     keywords='testing testautomation robotframework docker docker-compose',
     package_dir={'': 'src'},
     py_modules=['DockerComposeLibrary'],
     install_requires=[
-        'robotframework>=4,<6',
+        'robotframework>=4,<7',
         'packaging',
     ],
 )
```

### Comparing `robotframework-docker-1.4.0/src/DockerComposeLibrary.py` & `robotframework-docker-1.4.1/src/DockerComposeLibrary.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,18 +256,19 @@
 
         if no_deps:
             cmd.append('--no-deps')
 
         if force_recreate:
             cmd.append('--force-recreate')
 
-        if self._docker_compose_version < packaging.version.Version('1.19.0') and always_recreate_deps:
-            logger.warn('[Docker Compose Up] option --always-recreate-deps'
-                        f' is only supported since Docker Compose version v1.19.0'
-                        f' (using Docker Compose v{self._docker_compose_version})')
+        if self._docker_compose_version < packaging.version.Version('1.19.0'):
+            if always_recreate_deps:
+                logger.warn('[Docker Compose Up] option --always-recreate-deps'
+                            f' is only supported since Docker Compose version v1.19.0'
+                            f' (using Docker Compose v{self._docker_compose_version})')
         elif always_recreate_deps or always_recreate_deps is None:
             cmd.append('--always-recreate-deps')
 
         if no_recreate:
             cmd.append('--no-recreate')
 
         if no_build:
@@ -275,28 +276,30 @@
 
         if no_start:
             cmd.append('--no-start')
 
         if build:
             cmd.append('--build')
 
-        if self._docker_compose_version < packaging.version.Version('1.19.0') and renew_anon_volumes:
-            logger.warn('[Docker Compose Up] option --renew-anon-volumes'
-                        f' is only supported since Docker Compose version v1.19.0'
-                        f' (using Docker Compose v{self._docker_compose_version})')
+        if self._docker_compose_version < packaging.version.Version('1.19.0'):
+            if renew_anon_volumes:
+                logger.warn('[Docker Compose Up] option --renew-anon-volumes'
+                            f' is only supported since Docker Compose version v1.19.0'
+                            f' (using Docker Compose v{self._docker_compose_version})')
         elif renew_anon_volumes or renew_anon_volumes is None:
             cmd.append('--renew-anon-volumes')
 
         if remove_orphans:
             cmd.append('--remove-orphans')
 
-        if self._docker_compose_version < packaging.version.Version('2.0.0') and wait:
-            logger.warn('[Docker Compose Up] option --wait'
-                        f' is only supported since Docker Compose version v2.0.0'
-                        f' (using Docker Compose v{self._docker_compose_version})')
+        if self._docker_compose_version < packaging.version.Version('2.0.0'):
+            if wait:
+                logger.warn('[Docker Compose Up] option --wait'
+                            f' is only supported since Docker Compose version v2.0.0'
+                            f' (using Docker Compose v{self._docker_compose_version})')
         elif wait or wait is None:
             cmd.append('--wait')
 
         if service_names is not None:
             cmd.extend(service_names)
 
         try:
@@ -342,18 +345,19 @@
         Stop And Remove All Containers And Volumes
         | Docker Compose Down |
         """
 
         cmd: [str] = self._prepare_base_cmd()
         cmd.append('down')
 
-        if self._docker_compose_version < packaging.version.Version('1.18.0') and timeout is not None:
-            logger.warn('[Docker Compose Down] option --timeout'
-                        f' is only supported since Docker Compose version v1.18.0'
-                        f' (using Docker Compose v{self._docker_compose_version})')
+        if self._docker_compose_version < packaging.version.Version('1.18.0'):
+            if timeout is not None:
+                logger.warn('[Docker Compose Down] option --timeout'
+                            f' is only supported since Docker Compose version v1.18.0'
+                            f' (using Docker Compose v{self._docker_compose_version})')
         elif timeout is not None:
             cmd.append('--timeout')
             cmd.append(str(int(convert_time(timeout or '10 seconds'))))
 
         if rmi is not None:
             cmd.append('--rmi')
             cmd.append(rmi)
@@ -670,15 +674,15 @@
                                      cwd=self._project_directory,
                                      stdin=subprocess.DEVNULL,
                                      stdout=output_file,
                                      stderr=subprocess.PIPE,
                                      encoding=sys.getdefaultencoding(),
                                      text=True)
         except subprocess.CalledProcessError as e:
-            raise AssertionError(f'[Docker Compose Logs] Failed to get service logs: {e.stderr}') from e
+            raise AssertionError(f'[Docker Compose Logs] Failed to get service logs: {e.output.rstrip()}') from e
         finally:
             close_output_file()
 
         if write_to is None:
             return process.stdout
         return None
 
@@ -725,16 +729,16 @@
             output = subprocess.check_output(cmd,
                                              cwd=self._project_directory,
                                              stdin=subprocess.DEVNULL,
                                              stderr=subprocess.STDOUT,
                                              encoding=sys.getdefaultencoding(),
                                              text=True)
         except subprocess.CalledProcessError as e:
-            raise AssertionError(
-                f'[Get Exposed Service] Failed to query exposed ports for service {service_name}: {e.stderr}') from e
+            raise AssertionError(f'[Get Exposed Service] Failed to query exposed ports for service {service_name}:'
+                                 f' {e.output.rstrip()}') from e
 
         # Docker Compose V1 returns empty string when querying port that is not exposed.
         # Docker Compose V2 returns string ':0' in this case.
         result = output.rstrip().split(':')
         if len(result) != 2 or (result[0] == '' and result[1] == '0'):
             raise AssertionError(f'[Get Exposed Service] Port {port} is not exposed for service {service_name}')
```

### Comparing `robotframework-docker-1.4.0/src/robotframework_docker.egg-info/PKG-INFO` & `robotframework-docker-1.4.1/src/robotframework_docker.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: robotframework-docker
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Robot Framework Docker Library
 Home-page: https://github.com/vogoltsov/robotframework-docker
 Author: Vitaly Ogoltsov
 Author-email: vitaly.ogoltsov@me.com
 License: Apache License 2.0
 Keywords: testing testautomation robotframework docker docker-compose
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Robot Framework :: Library
 License-File: LICENSE
 
 Short Description
 -----------------
 
 `Robot Framework`_ library for working with ``docker`` and
```


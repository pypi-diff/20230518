# Comparing `tmp/sspqdd-1.0.7.tar.gz` & `tmp/sspqdd-4310105385.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspqdd-1.0.7.tar", last modified: Wed May 17 15:26:45 2023, max compression
+gzip compressed data, was "sspqdd-4310105385.tar", last modified: Thu May 18 16:02:01 2023, max compression
```

## Comparing `sspqdd-1.0.7.tar` & `sspqdd-4310105385.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 15:26:45.981384 sspqdd-1.0.7/
--rw-rw-rw-   0        0        0     1088 2023-05-17 15:26:45.981384 sspqdd-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6293 2023-04-14 13:52:05.000000 sspqdd-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 15:26:45.981384 sspqdd-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2358 2023-05-17 15:26:38.000000 sspqdd-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:26:45.964506 sspqdd-1.0.7/sspqdd/
--rw-rw-rw-   0        0        0        0 2023-05-17 10:19:04.000000 sspqdd-1.0.7/sspqdd/__init__.py
--rw-rw-rw-   0        0        0     3809 2023-05-17 11:25:56.000000 sspqdd-1.0.7/sspqdd/sspqdd_pkg.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:26:45.978912 sspqdd-1.0.7/sspqdd.egg-info/
--rw-rw-rw-   0        0        0     1088 2023-05-17 15:26:45.000000 sspqdd-1.0.7/sspqdd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-17 15:26:45.000000 sspqdd-1.0.7/sspqdd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 15:26:45.000000 sspqdd-1.0.7/sspqdd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 15:26:45.000000 sspqdd-1.0.7/sspqdd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:02:01.995602 sspqdd-4310105385/
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-05-18 16:02:01.995602 sspqdd-4310105385/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6201 2023-05-18 16:01:29.000000 sspqdd-4310105385/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 16:02:01.995602 sspqdd-4310105385/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-18 16:01:39.000000 sspqdd-4310105385/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:02:01.994602 sspqdd-4310105385/sspqdd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 16:01:39.000000 sspqdd-4310105385/sspqdd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3698 2023-05-18 16:01:39.000000 sspqdd-4310105385/sspqdd/sspqdd_pkg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:02:01.995602 sspqdd-4310105385/sspqdd.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-18 16:02:01.000000 sspqdd-4310105385/sspqdd.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-18 16:02:01.000000 sspqdd-4310105385/sspqdd.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-18 16:02:01.000000 sspqdd-4310105385/sspqdd.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-18 16:02:01.000000 sspqdd-4310105385/sspqdd.egg-info/top_level.txt
```

### Comparing `sspqdd-1.0.7/README.md` & `sspqdd-4310105385/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# SSPQDD
-
-
-
-## Getting started
-
-To make it easy for you to get started with GitLab, here's a list of recommended next steps.
-
-Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
-
-## Add your files
-
-- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
-
-```
-cd existing_repo
-git remote add origin https://gitlab.com/iturrinogarcia/sspqdd.git
-git branch -M main
-git push -uf origin main
-```
-
-## Integrate with your tools
-
-- [ ] [Set up project integrations](https://gitlab.com/iturrinogarcia/sspqdd/-/settings/integrations)
-
-## Collaborate with your team
-
-- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
-- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
-- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
-- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
-- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
-
-## Test and Deploy
-
-Use the built-in continuous integration in GitLab.
-
-- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
-- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
-- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
-- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
-- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
-
-***
-
-# Editing this README
-
-When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
-
-## Suggestions for a good README
-Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
-
-## Name
-Choose a self-explaining name for your project.
-
-## Description
-Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
-
-## Badges
-On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
-
-## Visuals
-Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
-
-## Installation
-Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
-
-## Usage
-Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
-
-## Support
-Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
-
-## Roadmap
-If you have ideas for releases in the future, it is a good idea to list them in the README.
-
-## Contributing
-State if you are open to contributions and what your requirements are for accepting them.
-
-For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
-
-You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
-
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
-
-## License
-For open source projects, say how it is licensed.
-
-## Project status
-If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+# SSPQDD
+
+
+
+## Getting started
+
+To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+
+Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+
+## Add your files
+
+- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
+- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+
+```
+cd existing_repo
+git remote add origin https://gitlab.com/iturrinogarcia/sspqdd.git
+git branch -M main
+git push -uf origin main
+```
+
+## Integrate with your tools
+
+- [ ] [Set up project integrations](https://gitlab.com/iturrinogarcia/sspqdd/-/settings/integrations)
+
+## Collaborate with your team
+
+- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
+- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
+- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
+- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
+- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+
+## Test and Deploy
+
+Use the built-in continuous integration in GitLab.
+
+- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
+- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
+- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
+- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
+- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+
+***
+
+# Editing this README
+
+When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
+
+## Suggestions for a good README
+Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
+
+## Name
+Choose a self-explaining name for your project.
+
+## Description
+Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
+
+## Badges
+On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
+
+## Visuals
+Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
+
+## Installation
+Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
+
+## Usage
+Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+
+## Support
+Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
+
+## Roadmap
+If you have ideas for releases in the future, it is a good idea to list them in the README.
+
+## Contributing
+State if you are open to contributions and what your requirements are for accepting them.
+
+For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
+
+You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
+
+## Authors and acknowledgment
+Show your appreciation to those who have contributed to the project.
+
+## License
+For open source projects, say how it is licensed.
+
+## Project status
+If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
```

### Comparing `sspqdd-1.0.7/setup.py` & `sspqdd-4310105385/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,39 @@
-from setuptools import setup
-
-setup(
-    name="sspqdd",
-    version="1.0.7",
-    description="Single-Shot-Power-Quality-Disturbance-Detector",
-    author="Carlos Iturrino-García",
-    author_email="carlos.iturrino.garcia@gmail.com",
-    packages=["sspqdd"],
-    long_description = "Single-Shot-Power-Quality-Disturbance-Detector (SSPQDD) is a Python package that provides a "
-                       "comprehensive solution for detection and"
-                       " classification of power quality disturbances. It utilizes state-of-the-art deep learning "
-                       "algorithms to analyze power signals and identify various types of disturbances, such as voltage"
-                       "sags, swells, harmonics, transients, notch and interruptions. The SSPQDD is designed to empower"
-                       " engineers and researchers working in the field of power quality analysis. By leveraging "
-                       "deep learning techniques, it offers an efficient and accurate approach to automatically detect "
-                       "and classify power disturbances, saving time and effort compared to manual inspection. "
-                       "With the SSPQDD, users can gain valuable insights into power quality issues and make informed "
-                       "decisions for optimal system performance and reliability.",
-    features = "\n - Detection and classification of power quality disturbances: SSPQDD provides an extensive library of "
-               "pre-trained deep learning models capable of identifying various power disturbances with high precision. "
-               "\n - Real-time monitoring: It enables real-time analysis of power signals,"
-               "allowing for immediate detection and notification of disturbances as they occur."
-               "\n - Customizability: Users have the flexibility to fine-tune or retrain the models with their "
-               "own datasets to cater to specific power quality analysis requirements. "
-               "\n -Visualization and reporting: PowerQDetect offers interactive visualization "
-               "tools and comprehensive reporting capabilities to help users interpret the detected disturbances "
-               "and generate detailed reports.",
-    # install_requires=[
-    #     "numpy",
-    #     "pandas",
-    # ],
+from setuptools import setup
+import os
+
+if os.environ.get('CI_COMMIT_TAG'):
+    version = os.environ['CI_COMMIT_TAG']
+else:
+    version = os.environ['CI_JOB_ID']
+
+setup(
+    name="sspqdd",
+    version=version,
+    description="Single-Shot-Power-Quality-Disturbance-Detector",
+    author="Carlos Iturrino-García",
+    author_email="carlos.iturrino.garcia@gmail.com",
+    packages=["sspqdd"],
+    long_description = "Single-Shot-Power-Quality-Disturbance-Detector (SSPQDD) is a Python package that provides a "
+                       "comprehensive solution for detection and"
+                       " classification of power quality disturbances. It utilizes state-of-the-art deep learning "
+                       "algorithms to analyze power signals and identify various types of disturbances, such as voltage"
+                       "sags, swells, harmonics, transients, notch and interruptions. The SSPQDD is designed to empower"
+                       " engineers and researchers working in the field of power quality analysis. By leveraging "
+                       "deep learning techniques, it offers an efficient and accurate approach to automatically detect "
+                       "and classify power disturbances, saving time and effort compared to manual inspection. "
+                       "With the SSPQDD, users can gain valuable insights into power quality issues and make informed "
+                       "decisions for optimal system performance and reliability.",
+    features = "\n - Detection and classification of power quality disturbances: SSPQDD provides an extensive library of "
+               "pre-trained deep learning models capable of identifying various power disturbances with high precision. "
+               "\n - Real-time monitoring: It enables real-time analysis of power signals,"
+               "allowing for immediate detection and notification of disturbances as they occur."
+               "\n - Customizability: Users have the flexibility to fine-tune or retrain the models with their "
+               "own datasets to cater to specific power quality analysis requirements. "
+               "\n -Visualization and reporting: PowerQDetect offers interactive visualization "
+               "tools and comprehensive reporting capabilities to help users interpret the detected disturbances "
+               "and generate detailed reports.",
+    # install_requires=[
+    #     "numpy",
+    #     "pandas",
+    # ],
 )
```

### Comparing `sspqdd-1.0.7/sspqdd/sspqdd_pkg.py` & `sspqdd-4310105385/sspqdd/sspqdd_pkg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import tensorflow as tf
-import numpy as np
-import matplotlib.pyplot as plt
-
-class SSPQDD(object):
-
-    def __init__(self):
-        self.model = tf.lite.Interpreter(model_path='./converted_model.tflite')
-        self.model.allocate_tensors()
-
-        self.input_details = self.model.get_input_details()
-        self.output_details = self.model.get_output_details()
-
-    def pre_process(self,sig,maxim,minim):
-
-        if len(sig) > 3000:
-            a = 0
-            b = 9
-            new = []
-            for i in range(3000):
-                window = sig[a:b]
-                new.append(np.max(window))
-                a += 10
-                b += 10
-        else:
-            new = sig
-        sig_norm = [(2/(maxim-minim))*new[i] for i in range(len(new))]
-        signal = np.array(sig_norm)
-
-        signal.shape=(tuple(self.input_details[0]['shape']))
-
-        return signal
-
-    def infer(self,sig,num_grid=188):
-        self.model.set_tensor(self.input_details[0]['index'], np.asarray(sig).astype('float32'))
-        self.model.invoke()
-
-        class_out = self.model.get_tensor(self.output_details[0]['index'])
-        conf_out = self.model.get_tensor(self.output_details[1]['index'])
-
-        pred_conf = np.array(tf.transpose(conf_out))
-        pred_conf.shape = (2, num_grid)
-        pred_class = np.array(tf.transpose(class_out))
-        pred_class.shape = (6, num_grid)
-
-        return pred_class,  pred_conf
-
-    def post_process(self,class_out,conf_out):
-        ind = [i for i, x in enumerate(conf_out[0]) if x > 0.9]
-        boxes = []
-        try:
-            start = ind[0]
-            # print(len(ind))
-            if len(ind) == 1:
-                block = {'start': (start * 16)-16,
-                         'stop': (start * 16)+16}
-                boxes.append(block)
-            else:
-                for i in range(len(ind) - 1):
-                    if ind[i + 1] - ind[i] == 1:
-                        block = {'start': start * 16,
-                                 'stop': ind[i + 1] * 16}
-                    elif ind[i + 1] - ind[i] != 1:
-                        boxes.append(block)
-                        start = ind[i + 1] * 16
-                boxes.append(block)
-
-            classi = class_out[:, ind[0]]
-            ind_class = np.argmax(classi)
-
-            return boxes, ind_class
-        except:
-
-            ind_class = []
-            return boxes, ind_class
-
-if __name__ == '__main__':
-    time = np.arange(0, 3.75, 1 / 8000)
-
-    amplitude = 10*np.sin(2 * 50 * np.pi * time)
-    amplitude[1600:1600 + 1600] = 1.5 * amplitude[1600:1600 + 1600]
-    # ind = 1600
-    # impulse = 9
-    # amplitude[ind] = impulse
-    sig = SSPQDD().pre_process(amplitude, 10, -10)
-    class_out, conf_out = SSPQDD().infer(sig)
-    boxes, ind_class = SSPQDD().post_process(class_out, conf_out)
-    #print(np.reshape(sig,(3000,)))
-    fig, axs = plt.subplots(2)
-    colors = ['red', 'blue', 'green', 'purple', 'orange', 'black']
-    axs[0].plot(10*np.reshape(sig,(3000,)))
-    axs[0].set_xlim([0, 3000])
-    axs[0].set_ylim([-15, 15])
-
-    for box in range(3):
-        rect = plt.Rectangle((boxes[0]['start'], 12.5), boxes[0]['stop'] - boxes[0]['start'], -25, linewidth=1,
-                             edgecolor=colors[ind_class], facecolor='none', zorder=2)
-        axs[0].add_patch(rect)
-    axs[1].plot(amplitude)
-    axs[1].set_xlim([0, len(amplitude)])
-    axs[1].set_ylim([-15, 15])
-    for box in range(3):
-        rect = plt.Rectangle((boxes[0]['start']*10, 12.5), boxes[0]['stop']*10 - boxes[0]['start']*10, -25, linewidth=1,
-                             edgecolor=colors[ind_class], facecolor='none', zorder=2)
-        axs[1].add_patch(rect)
-    plt.show()
-
+import tensorflow as tf
+import numpy as np
+import matplotlib.pyplot as plt
+
+class SSPQDD(object):
+
+    def __init__(self):
+        self.model = tf.lite.Interpreter(model_path='./converted_model.tflite')
+        self.model.allocate_tensors()
+
+        self.input_details = self.model.get_input_details()
+        self.output_details = self.model.get_output_details()
+
+    def pre_process(self,sig,maxim,minim):
+
+        if len(sig) > 3000:
+            a = 0
+            b = 9
+            new = []
+            for i in range(3000):
+                window = sig[a:b]
+                new.append(np.max(window))
+                a += 10
+                b += 10
+        else:
+            new = sig
+        sig_norm = [(2/(maxim-minim))*new[i] for i in range(len(new))]
+        signal = np.array(sig_norm)
+
+        signal.shape=(tuple(self.input_details[0]['shape']))
+
+        return signal
+
+    def infer(self,sig,num_grid=188):
+        self.model.set_tensor(self.input_details[0]['index'], np.asarray(sig).astype('float32'))
+        self.model.invoke()
+
+        class_out = self.model.get_tensor(self.output_details[0]['index'])
+        conf_out = self.model.get_tensor(self.output_details[1]['index'])
+
+        pred_conf = np.array(tf.transpose(conf_out))
+        pred_conf.shape = (2, num_grid)
+        pred_class = np.array(tf.transpose(class_out))
+        pred_class.shape = (6, num_grid)
+
+        return pred_class,  pred_conf
+
+    def post_process(self,class_out,conf_out):
+        ind = [i for i, x in enumerate(conf_out[0]) if x > 0.9]
+        boxes = []
+        try:
+            start = ind[0]
+            # print(len(ind))
+            if len(ind) == 1:
+                block = {'start': (start * 16)-16,
+                         'stop': (start * 16)+16}
+                boxes.append(block)
+            else:
+                for i in range(len(ind) - 1):
+                    if ind[i + 1] - ind[i] == 1:
+                        block = {'start': start * 16,
+                                 'stop': ind[i + 1] * 16}
+                    elif ind[i + 1] - ind[i] != 1:
+                        boxes.append(block)
+                        start = ind[i + 1] * 16
+                boxes.append(block)
+
+            classi = class_out[:, ind[0]]
+            ind_class = np.argmax(classi)
+
+            return boxes, ind_class
+        except:
+
+            ind_class = []
+            return boxes, ind_class
+
+if __name__ == '__main__':
+    time = np.arange(0, 3.75, 1 / 8000)
+
+    amplitude = 10*np.sin(2 * 50 * np.pi * time)
+    # amplitude[1600:1600 + 1600] = 1.5 * amplitude[1600:1600 + 1600]
+    ind = 1600
+    impulse = 9
+    amplitude[ind] = impulse
+    sig = SSPQDD().pre_process(amplitude, 10, -10)
+    class_out, conf_out = SSPQDD().infer(sig)
+    boxes, ind_class = SSPQDD().post_process(class_out, conf_out)
+    #print(np.reshape(sig,(3000,)))
+    fig, axs = plt.subplots(2)
+    colors = ['red', 'blue', 'green', 'purple', 'orange', 'black']
+    axs[0].plot(10*np.reshape(sig,(3000,)))
+    axs[0].set_xlim([0, 3000])
+    axs[0].set_ylim([-15, 15])
+
+    for box in range(3):
+        rect = plt.Rectangle((boxes[0]['start'], 12.5), boxes[0]['stop'] - boxes[0]['start'], -25, linewidth=1,
+                             edgecolor=colors[ind_class], facecolor='none', zorder=2)
+        axs[0].add_patch(rect)
+    axs[1].plot(amplitude)
+    axs[1].set_xlim([0, len(amplitude)])
+    axs[1].set_ylim([-15, 15])
+    for box in range(3):
+        rect = plt.Rectangle((boxes[0]['start']*10, 12.5), boxes[0]['stop']*10 - boxes[0]['start']*10, -25, linewidth=1,
+                             edgecolor=colors[ind_class], facecolor='none', zorder=2)
+        axs[1].add_patch(rect)
+    plt.show()
+
     print(boxes)
```


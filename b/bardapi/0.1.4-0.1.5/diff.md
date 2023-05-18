# Comparing `tmp/bardapi-0.1.4.tar.gz` & `tmp/bardapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bardapi-0.1.4.tar", last modified: Wed May 17 16:57:03 2023, max compression
+gzip compressed data, was "bardapi-0.1.5.tar", last modified: Thu May 18 02:59:24 2023, max compression
```

## Comparing `bardapi-0.1.4.tar` & `bardapi-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 16:57:03.783180 bardapi-0.1.4/
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     7849 2023-05-17 16:57:03.783180 bardapi-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6756 2023-05-17 16:42:09.000000 bardapi-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 16:57:03.772375 bardapi-0.1.4/bardapi/
--rw-rw-rw-   0        0        0      198 2023-05-17 16:42:20.000000 bardapi-0.1.4/bardapi/__init__.py
--rw-rw-rw-   0        0        0     3714 2023-05-17 16:54:40.000000 bardapi-0.1.4/bardapi/core.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:57:03.781145 bardapi-0.1.4/bardapi.egg-info/
--rw-rw-rw-   0        0        0     7849 2023-05-17 16:57:03.000000 bardapi-0.1.4/bardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-05-17 16:57:03.000000 bardapi-0.1.4/bardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:57:03.000000 bardapi-0.1.4/bardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 16:57:03.000000 bardapi-0.1.4/bardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 16:57:03.784625 bardapi-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1843 2023-05-17 16:56:55.000000 bardapi-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:59:24.365530 bardapi-0.1.5/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     7841 2023-05-18 02:59:24.362525 bardapi-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6748 2023-05-17 18:58:35.000000 bardapi-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 02:59:24.337369 bardapi-0.1.5/bardapi/
+-rw-rw-rw-   0        0        0      198 2023-05-18 02:59:01.000000 bardapi-0.1.5/bardapi/__init__.py
+-rw-rw-rw-   0        0        0     3714 2023-05-17 16:54:40.000000 bardapi-0.1.5/bardapi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:59:24.357525 bardapi-0.1.5/bardapi.egg-info/
+-rw-rw-rw-   0        0        0     7841 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 02:59:24.366529 bardapi-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1853 2023-05-18 02:58:49.000000 bardapi-0.1.5/setup.py
```

### Comparing `bardapi-0.1.4/LICENSE` & `bardapi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bardapi-0.1.4/PKG-INFO` & `bardapi-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bardapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: The python package that returns Response of Google Bard through API.
 Home-page: https://github.com/dsdanielpark/Bard-API
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -34,24 +34,24 @@
 <!-- <a href="https://pepy.tech/project/bardapi"><img alt="Downloads" src="https://pepy.tech/badge/bardapi"></a> -->
 <!-- <a><img alt="commit update" src="https://img.shields.io/github/last-commit/dsdanielpark/Bard-API?color=black"></a> -->
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://github.com/dsdanielpark/Bard-API"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false"/></a>
 <a href="https://pypi.org/project/bardapi/"><img alt="PyPI" src="https://img.shields.io/pypi/v/bardapi"></a>
 </p>
 
-> A package that returns Response of [Google Bard](https://bard.google.com/) through API
+> The python package that returns response of [Google Bard](https://bard.google.com/) through API.
 
 ![](./assets/bard_api.gif)
 
 
 I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). 
 
 <br>
 
-Never expose the `__Secure-1PSID` for your safety.
+Do not expose the `__Secure-1PSID`
 > Note that while I referred to `__Secure-1PSID` value as an API KEY for convenience, it is not an officially provided API KEY. 
 
 <br>
 
 ##  [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts) Is All You Need!
 - Helpful prompts for Google Bard
 
@@ -161,16 +161,16 @@
 <br>
 
 
 ## Scripts
 In the scripts [folder](./scripts/), I have released a script to help you compare [OpenAI-ChatGPT](./scripts/openai_api.ipynb) and [Google-Bard](./scripts/google_api.ipynb). I hope they will help more developers.
 
 ## License
-- [MIT](https://opensource.org/license/mit/) 
-- I hold no legal responsibility; for more information, please refer to the bottom of the readme file. I just want you to give me and [them](https://github.com/acheong08/Bard) a star...
+[MIT](https://opensource.org/license/mit/) <br>
+I hold no legal responsibility; for more information, please refer to the bottom of the readme file. I just want you to give me and [them](https://github.com/acheong08/Bard) a star.
 
 
 ## Bugs and Issues
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated.
 
 ## Contacts
 - Core maintainer: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.4 Summary: The python package
+Metadata-Version: 2.1 Name: bardapi Version: 0.1.5 Summary: The python package
 that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Natural Language :: Korean Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
@@ -17,25 +17,25 @@
 adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/
 68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667]
 Bard API
 [PyPI package]   [Code_style:_black] [https://hits.seeyoufarm.com/api/count/
 incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false]
 [PyPI]
-> A package that returns Response of [Google Bard](https://bard.google.com/
-) through API ![](./assets/bard_api.gif) I referred to [this github repository
-(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference
-process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask
-questions and get answers from Google Bard. This package is designed for
-application to the Python package [ExceptNotifier](https://github.com/
-dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-
-Coder).
-Never expose the `__Secure-1PSID` for your safety. > Note that while I referred
-to `__Secure-1PSID` value as an API KEY for convenience, it is not an
-officially provided API KEY.
+> The python package that returns response of [Google Bard](https://
+bard.google.com/) through API. ![](./assets/bard_api.gif) I referred to [this
+github repository(github.com/acheong08/Bard)](https://github.com/acheong08/
+Bard) where inference process of Bard was reverse engineered. Using `__Secure-
+1PSID`, you can ask questions and get answers from Google Bard. This package is
+designed for application to the Python package [ExceptNotifier](https://
+github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/
+dsdanielpark/Co-Coder).
+Do not expose the `__Secure-1PSID` > Note that while I referred to `__Secure-
+1PSID` value as an API KEY for convenience, it is not an officially provided
+API KEY.
 ## [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts)
 Is All You Need! - Helpful prompts for Google Bard
 ## Install The latest stable release (and required dependencies) can be
 installed from PyPI: ``` pip install bardapi ``` You may instead want to use
 the development version from Github: ``` pip install git+https://github.com/
 dsdanielpark/Bard-API.git ```
 ## Authentication 1. Visit https://bard.google.com/ 2. F12 for console 3.
@@ -73,20 +73,21 @@
 ["_BARD_API_KEY"]) bard = Bard(session=session) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
 Simple Example
 [./assets/bardimg.png]_
 ##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
 help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
 (./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
--_[MIT](https://opensource.org/license/mit/)_-_I_hold_no_legal_responsibility;
-for_more_information,_please_refer_to_the_bottom_of_the_readme_file._I_just
-want_you_to_give_me_and_[them](https://github.com/acheong08/Bard)_a_star..._##
-Bugs_and_Issues_Sincerely_grateful_for_any_reports_on_new_features_or_bugs.
-Your_valuable_feedback_on_the_code_is_highly_appreciated._##_Contacts_-_Core
-maintainer:_[Daniel_Park,_South_Korea](https://github.com/DSDanielPark)_
+[MIT](https://opensource.org/license/mit/)_
+I_hold_no_legal_responsibility;_for_more_information,_please_refer_to_the
+bottom_of_the_readme_file._I_just_want_you_to_give_me_and_[them](https://
+github.com/acheong08/Bard)_a_star._##_Bugs_and_Issues_Sincerely_grateful_for
+any_reports_on_new_features_or_bugs._Your_valuable_feedback_on_the_code_is
+highly_appreciated._##_Contacts_-_Core_maintainer:_[Daniel_Park,_South_Korea]
+(https://github.com/DSDanielPark)_
 -_E-mail:_parkminwoo1991@gmail.com_
 ##_Reference_[1]_https://github.com/acheong08/Bard_###_Important_Notice_The
 user_assumes_all_legal_responsibilities_associated_with_using_the_BardAPI
 package._This_Python_package_merely_facilitates_easy_access_to_Google_Bard_for
 developers._Users_are_solely_responsible_for_managing_data_and_using_the
 package_appropriately._For_further_information,_please_consult_the_Google_Bard
 Official_Document._####_Could_you_kindly_add_this_badge_to_your_repository?
```

### Comparing `bardapi-0.1.4/README.md` & `bardapi-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 <!-- <a href="https://pepy.tech/project/bardapi"><img alt="Downloads" src="https://pepy.tech/badge/bardapi"></a> -->
 <!-- <a><img alt="commit update" src="https://img.shields.io/github/last-commit/dsdanielpark/Bard-API?color=black"></a> -->
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://github.com/dsdanielpark/Bard-API"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false"/></a>
 <a href="https://pypi.org/project/bardapi/"><img alt="PyPI" src="https://img.shields.io/pypi/v/bardapi"></a>
 </p>
 
-> A package that returns Response of [Google Bard](https://bard.google.com/) through API
+> The python package that returns response of [Google Bard](https://bard.google.com/) through API.
 
 ![](./assets/bard_api.gif)
 
 
 I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). 
 
 <br>
 
-Never expose the `__Secure-1PSID` for your safety.
+Do not expose the `__Secure-1PSID`
 > Note that while I referred to `__Secure-1PSID` value as an API KEY for convenience, it is not an officially provided API KEY. 
 
 <br>
 
 ##  [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts) Is All You Need!
 - Helpful prompts for Google Bard
 
@@ -136,16 +136,16 @@
 <br>
 
 
 ## Scripts
 In the scripts [folder](./scripts/), I have released a script to help you compare [OpenAI-ChatGPT](./scripts/openai_api.ipynb) and [Google-Bard](./scripts/google_api.ipynb). I hope they will help more developers.
 
 ## License
-- [MIT](https://opensource.org/license/mit/) 
-- I hold no legal responsibility; for more information, please refer to the bottom of the readme file. I just want you to give me and [them](https://github.com/acheong08/Bard) a star...
+[MIT](https://opensource.org/license/mit/) <br>
+I hold no legal responsibility; for more information, please refer to the bottom of the readme file. I just want you to give me and [them](https://github.com/acheong08/Bard) a star.
 
 
 ## Bugs and Issues
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated.
 
 ## Contacts
 - Core maintainer: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
```

#### html2text {}

```diff
@@ -3,25 +3,25 @@
 adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/
 68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667]
 Bard API
 [PyPI package]   [Code_style:_black] [https://hits.seeyoufarm.com/api/count/
 incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false]
 [PyPI]
-> A package that returns Response of [Google Bard](https://bard.google.com/
-) through API ![](./assets/bard_api.gif) I referred to [this github repository
-(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference
-process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask
-questions and get answers from Google Bard. This package is designed for
-application to the Python package [ExceptNotifier](https://github.com/
-dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-
-Coder).
-Never expose the `__Secure-1PSID` for your safety. > Note that while I referred
-to `__Secure-1PSID` value as an API KEY for convenience, it is not an
-officially provided API KEY.
+> The python package that returns response of [Google Bard](https://
+bard.google.com/) through API. ![](./assets/bard_api.gif) I referred to [this
+github repository(github.com/acheong08/Bard)](https://github.com/acheong08/
+Bard) where inference process of Bard was reverse engineered. Using `__Secure-
+1PSID`, you can ask questions and get answers from Google Bard. This package is
+designed for application to the Python package [ExceptNotifier](https://
+github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/
+dsdanielpark/Co-Coder).
+Do not expose the `__Secure-1PSID` > Note that while I referred to `__Secure-
+1PSID` value as an API KEY for convenience, it is not an officially provided
+API KEY.
 ## [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts)
 Is All You Need! - Helpful prompts for Google Bard
 ## Install The latest stable release (and required dependencies) can be
 installed from PyPI: ``` pip install bardapi ``` You may instead want to use
 the development version from Github: ``` pip install git+https://github.com/
 dsdanielpark/Bard-API.git ```
 ## Authentication 1. Visit https://bard.google.com/ 2. F12 for console 3.
@@ -59,20 +59,21 @@
 ["_BARD_API_KEY"]) bard = Bard(session=session) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
 Simple Example
 [./assets/bardimg.png]_
 ##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
 help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
 (./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
--_[MIT](https://opensource.org/license/mit/)_-_I_hold_no_legal_responsibility;
-for_more_information,_please_refer_to_the_bottom_of_the_readme_file._I_just
-want_you_to_give_me_and_[them](https://github.com/acheong08/Bard)_a_star..._##
-Bugs_and_Issues_Sincerely_grateful_for_any_reports_on_new_features_or_bugs.
-Your_valuable_feedback_on_the_code_is_highly_appreciated._##_Contacts_-_Core
-maintainer:_[Daniel_Park,_South_Korea](https://github.com/DSDanielPark)_
+[MIT](https://opensource.org/license/mit/)_
+I_hold_no_legal_responsibility;_for_more_information,_please_refer_to_the
+bottom_of_the_readme_file._I_just_want_you_to_give_me_and_[them](https://
+github.com/acheong08/Bard)_a_star._##_Bugs_and_Issues_Sincerely_grateful_for
+any_reports_on_new_features_or_bugs._Your_valuable_feedback_on_the_code_is
+highly_appreciated._##_Contacts_-_Core_maintainer:_[Daniel_Park,_South_Korea]
+(https://github.com/DSDanielPark)_
 -_E-mail:_parkminwoo1991@gmail.com_
 ##_Reference_[1]_https://github.com/acheong08/Bard_###_Important_Notice_The
 user_assumes_all_legal_responsibilities_associated_with_using_the_BardAPI
 package._This_Python_package_merely_facilitates_easy_access_to_Google_Bard_for
 developers._Users_are_solely_responsible_for_managing_data_and_using_the
 package_appropriately._For_further_information,_please_consult_the_Google_Bard
 Official_Document._####_Could_you_kindly_add_this_badge_to_your_repository?
```

### Comparing `bardapi-0.1.4/bardapi/core.py` & `bardapi-0.1.5/bardapi/core.py`

 * *Files identical despite different names*

### Comparing `bardapi-0.1.4/bardapi.egg-info/PKG-INFO` & `bardapi-0.1.5/bardapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bardapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: The python package that returns Response of Google Bard through API.
 Home-page: https://github.com/dsdanielpark/Bard-API
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -34,24 +34,24 @@
 <!-- <a href="https://pepy.tech/project/bardapi"><img alt="Downloads" src="https://pepy.tech/badge/bardapi"></a> -->
 <!-- <a><img alt="commit update" src="https://img.shields.io/github/last-commit/dsdanielpark/Bard-API?color=black"></a> -->
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://github.com/dsdanielpark/Bard-API"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false"/></a>
 <a href="https://pypi.org/project/bardapi/"><img alt="PyPI" src="https://img.shields.io/pypi/v/bardapi"></a>
 </p>
 
-> A package that returns Response of [Google Bard](https://bard.google.com/) through API
+> The python package that returns response of [Google Bard](https://bard.google.com/) through API.
 
 ![](./assets/bard_api.gif)
 
 
 I referred to [this github repository(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask questions and get answers from Google Bard. This package is designed for application to the Python package [ExceptNotifier](https://github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-Coder). 
 
 <br>
 
-Never expose the `__Secure-1PSID` for your safety.
+Do not expose the `__Secure-1PSID`
 > Note that while I referred to `__Secure-1PSID` value as an API KEY for convenience, it is not an officially provided API KEY. 
 
 <br>
 
 ##  [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts) Is All You Need!
 - Helpful prompts for Google Bard
 
@@ -161,16 +161,16 @@
 <br>
 
 
 ## Scripts
 In the scripts [folder](./scripts/), I have released a script to help you compare [OpenAI-ChatGPT](./scripts/openai_api.ipynb) and [Google-Bard](./scripts/google_api.ipynb). I hope they will help more developers.
 
 ## License
-- [MIT](https://opensource.org/license/mit/) 
-- I hold no legal responsibility; for more information, please refer to the bottom of the readme file. I just want you to give me and [them](https://github.com/acheong08/Bard) a star...
+[MIT](https://opensource.org/license/mit/) <br>
+I hold no legal responsibility; for more information, please refer to the bottom of the readme file. I just want you to give me and [them](https://github.com/acheong08/Bard) a star.
 
 
 ## Bugs and Issues
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated.
 
 ## Contacts
 - Core maintainer: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.4 Summary: The python package
+Metadata-Version: 2.1 Name: bardapi Version: 0.1.5 Summary: The python package
 that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Natural Language :: Korean Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
@@ -17,25 +17,25 @@
 adb54264fe2ad5067d07d0752fc32600b4e6250073b01ce8c386575b431e3f06/
 68747470733a2f2f7777772e677374617469632e636f6d2f6c616d64612f696d616765732f66617669636f6e5f76315f31353031363063646466663766323934636533302e737667]
 Bard API
 [PyPI package]   [Code_style:_black] [https://hits.seeyoufarm.com/api/count/
 incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FBARD_API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=BardAPI&edge_flat=false]
 [PyPI]
-> A package that returns Response of [Google Bard](https://bard.google.com/
-) through API ![](./assets/bard_api.gif) I referred to [this github repository
-(github.com/acheong08/Bard)](https://github.com/acheong08/Bard) where inference
-process of Bard was reverse engineered. Using `__Secure-1PSID`, you can ask
-questions and get answers from Google Bard. This package is designed for
-application to the Python package [ExceptNotifier](https://github.com/
-dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/dsdanielpark/Co-
-Coder).
-Never expose the `__Secure-1PSID` for your safety. > Note that while I referred
-to `__Secure-1PSID` value as an API KEY for convenience, it is not an
-officially provided API KEY.
+> The python package that returns response of [Google Bard](https://
+bard.google.com/) through API. ![](./assets/bard_api.gif) I referred to [this
+github repository(github.com/acheong08/Bard)](https://github.com/acheong08/
+Bard) where inference process of Bard was reverse engineered. Using `__Secure-
+1PSID`, you can ask questions and get answers from Google Bard. This package is
+designed for application to the Python package [ExceptNotifier](https://
+github.com/dsdanielpark/ExceptNotifier) and [Co-Coder](https://github.com/
+dsdanielpark/Co-Coder).
+Do not expose the `__Secure-1PSID` > Note that while I referred to `__Secure-
+1PSID` value as an API KEY for convenience, it is not an officially provided
+API KEY.
 ## [Amazing Bard Prompts](https://github.com/dsdanielpark/amazing-bard-prompts)
 Is All You Need! - Helpful prompts for Google Bard
 ## Install The latest stable release (and required dependencies) can be
 installed from PyPI: ``` pip install bardapi ``` You may instead want to use
 the development version from Github: ``` pip install git+https://github.com/
 dsdanielpark/Bard-API.git ```
 ## Authentication 1. Visit https://bard.google.com/ 2. F12 for console 3.
@@ -73,20 +73,21 @@
 ["_BARD_API_KEY"]) bard = Bard(session=session) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
 Simple Example
 [./assets/bardimg.png]_
 ##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
 help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
 (./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
--_[MIT](https://opensource.org/license/mit/)_-_I_hold_no_legal_responsibility;
-for_more_information,_please_refer_to_the_bottom_of_the_readme_file._I_just
-want_you_to_give_me_and_[them](https://github.com/acheong08/Bard)_a_star..._##
-Bugs_and_Issues_Sincerely_grateful_for_any_reports_on_new_features_or_bugs.
-Your_valuable_feedback_on_the_code_is_highly_appreciated._##_Contacts_-_Core
-maintainer:_[Daniel_Park,_South_Korea](https://github.com/DSDanielPark)_
+[MIT](https://opensource.org/license/mit/)_
+I_hold_no_legal_responsibility;_for_more_information,_please_refer_to_the
+bottom_of_the_readme_file._I_just_want_you_to_give_me_and_[them](https://
+github.com/acheong08/Bard)_a_star._##_Bugs_and_Issues_Sincerely_grateful_for
+any_reports_on_new_features_or_bugs._Your_valuable_feedback_on_the_code_is
+highly_appreciated._##_Contacts_-_Core_maintainer:_[Daniel_Park,_South_Korea]
+(https://github.com/DSDanielPark)_
 -_E-mail:_parkminwoo1991@gmail.com_
 ##_Reference_[1]_https://github.com/acheong08/Bard_###_Important_Notice_The
 user_assumes_all_legal_responsibilities_associated_with_using_the_BardAPI
 package._This_Python_package_merely_facilitates_easy_access_to_Google_Bard_for
 developers._Users_are_solely_responsible_for_managing_data_and_using_the
 package_appropriately._For_further_information,_please_consult_the_Google_Bard
 Official_Document._####_Could_you_kindly_add_this_badge_to_your_repository?
```

### Comparing `bardapi-0.1.4/setup.py` & `bardapi-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
 
 version = get_version()
 
 
 setup(
     name="bardapi",
-    version="0.1.4",
+    version="0.1.5",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="The python package that returns Response of Google Bard through API.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/Bard-API",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=[],
+    install_requires=["requests"],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Natural Language :: Korean",
         "Programming Language :: Python",
```


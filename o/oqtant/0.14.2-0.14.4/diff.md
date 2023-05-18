# Comparing `tmp/oqtant-0.14.2.tar.gz` & `tmp/oqtant-0.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqtant-0.14.2.tar", max compression
+gzip compressed data, was "oqtant-0.14.4.tar", max compression
```

## Comparing `oqtant-0.14.2.tar` & `oqtant-0.14.4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    11341 2023-01-20 21:46:26.574896 oqtant-0.14.2/LICENSE
--rw-r--r--   0        0        0     2434 2023-05-08 19:04:48.398282 oqtant-0.14.2/README.md
--rw-r--r--   0        0        0     8556 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/INSTALL.md
--rw-r--r--   0        0        0     4436 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/albert_api_docs.md
--rw-r--r--   0        0        0    10947 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/job_analysis_docs.md
--rw-r--r--   0        0        0    26364 2023-05-02 19:38:25.421229 oqtant-0.14.2/documentation/main.css
--rw-r--r--   0        0        0    10316 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/oqtant_api_docs.md
--rw-r--r--   0        0        0    15152 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_1_bec_jobs.ipynb
--rw-r--r--   0        0        0     9895 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_1_bec_jobs.md
--rw-r--r--   0        0        0    14537 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_2_barrier_jobs.ipynb
--rw-r--r--   0        0        0     9553 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_2_barrier_jobs.md
--rw-r--r--   0        0        0    31799 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_3_abstractions.ipynb
--rw-r--r--   0        0        0    21970 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_3_abstractions.md
--rw-r--r--   0        0        0    13266 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_4_experiment.ipynb
--rw-r--r--   0        0        0     9097 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_4_experiment.md
--rw-r--r--   0        0        0    16999 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_5_optimization.ipynb
--rw-r--r--   0        0        0    11308 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_5_optimization.md
--rw-r--r--   0        0        0      463 2023-05-04 14:03:20.362947 oqtant-0.14.2/documentation/tutorials/tutorials.md
--rw-r--r--   0        0        0        0 2023-05-05 20:25:04.057852 oqtant-0.14.2/oqtant/__init__.py
--rw-r--r--   0        0        0    21848 2023-05-08 14:41:12.223285 oqtant-0.14.2/oqtant/oqtant_client.py
--rw-r--r--   0        0        0        0 2023-05-05 20:25:04.057852 oqtant-0.14.2/oqtant/schemas/__init__.py
--rw-r--r--   0        0        0    17813 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/schemas/job.py
--rw-r--r--   0        0        0     1002 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/settings.py
--rw-r--r--   0        0        0        0 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/util/__init__.py
--rw-r--r--   0        0        0     2805 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/util/auth.py
--rw-r--r--   0        0        0     1023 2023-05-08 14:41:12.223285 oqtant-0.14.2/oqtant/util/exceptions.py
--rw-r--r--   0        0        0      474 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/util/server.py
--rw-r--r--   0        0        0     3181 2023-05-08 19:05:24.786316 oqtant-0.14.2/pyproject.toml
--rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 oqtant-0.14.2/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-05-18 18:21:57.682992 oqtant-0.14.4/LICENSE
+-rw-r--r--   0        0        0     2458 2023-05-18 18:25:51.795428 oqtant-0.14.4/README.md
+-rw-r--r--   0        0        0     7953 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/INSTALL.md
+-rw-r--r--   0        0        0     4436 2023-05-18 18:23:47.003196 oqtant-0.14.4/documentation/albert_api_docs.md
+-rw-r--r--   0        0        0    10947 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/job_analysis_docs.md
+-rw-r--r--   0        0        0    26364 2023-05-18 18:21:57.682992 oqtant-0.14.4/documentation/main.css
+-rw-r--r--   0        0        0     4436 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/oqtant_api_docs.md
+-rw-r--r--   0        0        0    10316 2023-05-18 18:23:54.771210 oqtant-0.14.4/documentation/oqtant_client_docs.md
+-rw-r--r--   0        0        0    15152 2023-05-18 18:27:49.315647 oqtant-0.14.4/documentation/tutorials/tutorial_1_bec_jobs.ipynb
+-rw-r--r--   0        0        0     9895 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/tutorials/tutorial_1_bec_jobs.md
+-rw-r--r--   0        0        0    14537 2023-05-18 18:27:49.311647 oqtant-0.14.4/documentation/tutorials/tutorial_2_barrier_jobs.ipynb
+-rw-r--r--   0        0        0     9553 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/tutorials/tutorial_2_barrier_jobs.md
+-rw-r--r--   0        0        0    31799 2023-05-18 18:27:49.343647 oqtant-0.14.4/documentation/tutorials/tutorial_3_abstractions.ipynb
+-rw-r--r--   0        0        0    21972 2023-05-18 18:26:15.187472 oqtant-0.14.4/documentation/tutorials/tutorial_3_abstractions.md
+-rw-r--r--   0        0        0    13266 2023-05-18 18:27:49.347647 oqtant-0.14.4/documentation/tutorials/tutorial_4_experiment.ipynb
+-rw-r--r--   0        0        0     9097 2023-05-18 18:26:15.191472 oqtant-0.14.4/documentation/tutorials/tutorial_4_experiment.md
+-rw-r--r--   0        0        0    16999 2023-05-18 18:27:49.311647 oqtant-0.14.4/documentation/tutorials/tutorial_5_optimization.ipynb
+-rw-r--r--   0        0        0    11308 2023-05-18 18:26:15.191472 oqtant-0.14.4/documentation/tutorials/tutorial_5_optimization.md
+-rw-r--r--   0        0        0      463 2023-05-18 18:26:15.191472 oqtant-0.14.4/documentation/tutorials/tutorials.md
+-rw-r--r--   0        0        0        0 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/__init__.py
+-rw-r--r--   0        0        0    21848 2023-05-18 18:26:26.755493 oqtant-0.14.4/oqtant/oqtant_client.py
+-rw-r--r--   0        0        0        0 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/schemas/__init__.py
+-rw-r--r--   0        0        0    17813 2023-05-18 18:26:26.755493 oqtant-0.14.4/oqtant/schemas/job.py
+-rw-r--r--   0        0        0     1002 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/settings.py
+-rw-r--r--   0        0        0        0 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/util/__init__.py
+-rw-r--r--   0        0        0     2805 2023-05-18 18:26:26.759493 oqtant-0.14.4/oqtant/util/auth.py
+-rw-r--r--   0        0        0     1023 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/util/exceptions.py
+-rw-r--r--   0        0        0      474 2023-05-18 18:21:57.682992 oqtant-0.14.4/oqtant/util/server.py
+-rw-r--r--   0        0        0     3203 2023-05-18 18:26:45.991529 oqtant-0.14.4/pyproject.toml
+-rw-r--r--   0        0        0     3739 1970-01-01 00:00:00.000000 oqtant-0.14.4/PKG-INFO
```

### Comparing `oqtant-0.14.2/LICENSE` & `oqtant-0.14.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.2/README.md` & `oqtant-0.14.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -11,46 +11,46 @@
 pip install oqtant
 ```
 
 ## 🧭 Introduction
 
 This API contains tools to:
 
-- Access all the functionality of the Albert Web App (https://albert.coldquanta.com)
+- Access all the functionality of the Albert Web App (https://albert-dev.coldquanta.com)
 
   - BARRIER (Barrier Manipulator) jobs
   - BEC (Ultracold Matter) jobs
 
-- Build parameterized (i.e. optimization) experiments using AlbertJobs
+- Build parameterized (i.e. optimization) experiments using OqtantJobs
 
-- Submit and retrieve AlbertJob results
+- Submit and retrieve OqtantJob results
 
 ## 🤖 How Oqtant Works
 
-- Construct a single or list of jobs using the AlbertJob class
+- Construct a single or list of jobs using the OqtantJob class
 
   - 1D parameter sweeps are supported
 
 - Run a single or list of jobs using run_jobs(). The jobs are submitted to run on hardware in FIFO queue.
 
   - job lists are run sequentially (uninterrupted) unless list exceeds 30 jobs
 
-- As jobs run, AlbertJob objects are created automatically and stored in active_jobs.
+- As jobs run, OqtantJob objects are created automatically and stored in active_jobs.
 
   - View these jobs with see_active_jobs()
   - These jobs are available until the python session ends.
 
 - To operate on jobs from a current or previous session, load them into active_jobs with
 
   - load_job_from_id(), load_job_from_id_list(), load_job_from_file(), load_job_from_file_list()
 
-- To analyze job objects and use Albert's job analysis library, reference the AlbertJob class documentation.
+- To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.
 
 Need help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!
 
 ## 📓 Documentation
 
-- [Getting started](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/INSTALL.md) (installation, setting up the environment, How to run the tutorial notebooks)
-- [Tutorials](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/tutorials/tutorials.md) (demos for creating and submitting jobs)
-- [Oqtant API docs](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/oqtant_api_docs.md)
-- [Albert API docs](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/albert_api_docs.md)
-- [Job Analysis docs](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/job_analysis_docs.md)
+- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, How to run the tutorial notebooks)
+- [Tutorials](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/tutorials/tutorials.md) (demos for creating and submitting jobs)
+- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oqtant_api_docs.md)
+- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/albert_api_docs.md)
+- [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)
```

### Comparing `oqtant-0.14.2/documentation/INSTALL.md` & `oqtant-0.14.4/documentation/INSTALL.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Oqtant Quickstart Guide
 
 To get started with Oqtant you will need to have the following installed:
 
 - Python >=3.10 and <3.12
 
+# User Account
+
+You will need to have a registered Explorer account, available at https://albert-dev.coldquanta.com.
+
 # Installation
 
 Oqtant is compatible with Windows, Mac and Linux. Below are the steps needed to get Oqtant installed with instructions for each operating system
 
 ## Python + Pip
 
 If you do not already have a compatible version of python and pip installed on your system follow the instructions below:
@@ -103,19 +107,17 @@
    ```
 
    Replace `<path to virtual environment location>` with where the virtual environment was created. The path should include the name of the virtual environment, in this case we used `.venv`
 
 3. Inside of the activated virtual environment run the following command to install Oqtant and it's dependencies:
 
    ```
-   pip install <path to file location>\oqtant-<oqtant version>-py3-none-any.whl
+   pip install oqtant
    ```
 
-   Replace `<path to file location>` with where the downloaded .whl file is located on your system. Replace `<oqtant version>` with the version of Oqtant you have downloaded, it should look something like this: `oqtant-0.0.0-py3-none-any.whl`
-
 ### Linux/Mac
 
 1. Create a python virtual environment to install Oqtant into:
 
    ```
    python -m venv .venv
    ```
@@ -129,41 +131,47 @@
    ```
 
    Replace `<path to virtual environment location>` with where the virtual environment was created. The path should include the name of the virtual environment, in this case we used `.venv`
 
 3. Once activated run the following command to install Oqtant and it's dependencies:
 
    ```
-   pip install <path to file location>/oqtant-<oqtant version>-py3-none-any.whl
+   pip install oqtant
    ```
 
-Replace `<path to file location>` with where the downloaded .whl file is located on your system. Replace `<oqtant version>` with the version of Oqtant you have downloaded, it should look something like this: `oqtant-0.1.0-py3-none-any.whl`
-
 # Tutorial Notebooks
 
-Getting started with Oqtant is easy using the tutorial notebooks (your Oqtant installation already includes the latest version of Jupyter Notebook). These tutorials will walk you through the basic functions of using Oqtant to interact with the Albert hardware. Feel free to use these as a starting point for your own code: edit, rename, share… they are yours.
+Getting started with Oqtant is easy using the tutorial notebooks (your Oqtant installation already includes the latest version of Jupyter Notebook). These tutorials will walk you through the basic functions of using Oqtant to interact with the Oqtant hardware. Feel free to use these as a starting point for your own code: edit, rename, share… they are yours.
 
-## Running Tutorial Notebooks
+## Downloading Tutorial Notebooks
 
-Once Oqtant and it's dependencies have successfully been installed into your python virtual environment you can now open and use the provided tutorial notebooks. If you downloaded Oqtant from [https://albert-dev.coldquanta.com](https://albert-dev.coldquanta.com) you can find the tutorial notebooks inside of the same folder as the Oqtant `.whl` file in the `documentation/tutorials` folder. There is also an option to download the tutorial notebooks on their own here [https://albert-dev.coldquanta.com/resources](https://albert-dev.coldquanta.com/resources)
+You can download a copy of our tutorial notebooks from our GitLab project located here: TODO
 
-To start up Jupyter and begin using the tutorial notebooks run the following command in the same directory as the notebook files:
+## Running Tutorial Notebooks
+
+To start up Jupyter and begin using the tutorial notebooks run the following command in the same directory as the notebook files you have downloaded:
 
 ```
 jupyter notebook
 ```
 
 - This will open a tab in your default web browser with a file explorer type interface.
 - Using this interface navigate to the location of the provided notebooks and select one to open.
 - This will open another tab with the contents of the selected notebook.
 - Each notebook has pre-populated examples you can then execute with instructions for each step
 - For a more detailed explanation of the Oqtant API refer to our [API Docs](oqtant_api_docs.md)
 
+If you run into `ModuleNotFound` errors when running cells within the notebooks it can be a sign that the notebooks are not using the correct version of python. To fix this close the notebook server, run the following, then restart the notebooks:
+
+```
+python -m ipykernel install --user
+```
+
 **Note: You may notice that each tutorial notebook has two files with different extensions (.ipynb and .md). The files you want to be using with Jupyter are the .ipynb files as these are what runs the underlying Oqtant python code. The .md files are static markdown representations of the tutorial notebooks that can be used as reference if needed. The .md files are safe to delete**
 
 ## Authentication
 
-At the top of each tutorial notebook you will see a step called `Sign into Albert`. This step is required for all notebook and client operations to ensure only authorized parties are accessing Albert.
+At the top of each tutorial notebook you will see a step called `Sign into Oqtant`. This step is required for all notebook and client operations to ensure only authorized parties are accessing Oqtant.
 
-This step will require that you already have an account created for Albert. If you have not done so yet visit https://albert-dev.coldquanta.com and follow the registration steps to get set up.
+This step will require that you already have an account created for Oqtant. If you have not done so yet visit https://albert-dev.coldquanta.com and follow the registration steps to get set up.
 
 <link href="main.css" rel="stylesheet" />
```

### Comparing `oqtant-0.14.2/documentation/albert_api_docs.md` & `oqtant-0.14.4/documentation/albert_api_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.2/documentation/job_analysis_docs.md` & `oqtant-0.14.4/documentation/job_analysis_docs.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 ## Capabilities
 
 - Contains job inputs and outputs (if they exist) as well as information about the user, hardware, and submission time.
 - Analysis functions for TOF images and some convenient output/plotting utilities
 
 ## How the BEC Job Analysis Library works
 
-1. A AlbertJob is a container object for inputs and results generated by the Albert system.
-   The AlbertJob object has a variety of common utility functions for processing results.
+1. A OqtantJob is a container object for inputs and results generated by the Oqtant system.
+   The OqtantJob object has a variety of common utility functions for processing results.
 
-2. Within a Oqtant session, AlbertJob objects are created and stored in active_jobs.
+2. Within a Oqtant session, OqtantJob objects are created and stored in active_jobs.
    These jobs are available until the python session ends. All jobs are tracked by their id,
    which is issued at the time of job submit.
 
 3. To handle job results from a previous session, load them into active_jobs with
-   load_job_from_id() or load_job_from_file(). This will create the AlbertJob object(s).
+   load_job_from_id() or load_job_from_file(). This will create the OqtantJob object(s).
 
-4. Each AlbertJob object has a status assigned by the Albert hardware:
+4. Each OqtantJob object has a status assigned by the Oqtant hardware:
    - Pending - This job has not run yet. No results available
    - Running - This job is being evaluated. Run time is 1 minute.
    - Complete - This job has run successfully and results are available.
    - Failed - This job has failed. This can occur due to inappropriate input parameters or
      hardware outages. Contact **albert@infleqtion.com** for support
 
 ## Helper functions
@@ -120,18 +120,18 @@
     :param os:
     :type os: float - Constant offset
 
     returns array sampled OD, sum of 2d gaussian distribution and TF distribution. flattened to 1D
 
 ## BEC_job class
 
-This is a container class for an Albert job in any state
+This is a container class for an Oqtant job in any state
 
-A AlbertJob object contains job parameters and results (if they have been generated).
-The AlbertJob class contains analysis functions to apply to TOF images.
+A OqtantJob object contains job parameters and results (if they have been generated).
+The OqtantJob class contains analysis functions to apply to TOF images.
 
 ### init
 
     :param job_dict:
     :type job_dict: dict - valid dictionary of job inputs used to submit the job to run on hardware
 
     attributes:
```

### Comparing `oqtant-0.14.2/documentation/main.css` & `oqtant-0.14.4/documentation/main.css`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.2/documentation/oqtant_api_docs.md` & `oqtant-0.14.4/documentation/oqtant_client_docs.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # Oqtant Client
 
 ## Capabilities
 
-- Access all the functionality of the Albert Web App (https://albert-dev.coldquanta.com)
+- Access all the functionality of the Oqtant Web App (https://albert-dev.coldquanta.com)
 
   - BARRIER (Barrier Manipulator) jobs
   - BEC (Ultracold Matter) jobs
 
-- Build parameterized (i.e. optimization) experiments using AlbertJobs
+- Build parameterized (i.e. optimization) experiments using OqtantJobs
 
-- Submit and retrieve AlbertJob results
+- Submit and retrieve OqtantJob results
 
 ## How Oqtant Works
 
-- Construct a single or list of jobs using the AlbertJob class
+- Construct a single or list of jobs using the OqtantJob class
 
   - 1D parameter sweeps are supported
 
 - Run a single or list of jobs using run_jobs(). The jobs are submitted to run on hardware in FIFO queue.
 
   - job lists are run sequentially (uninterrupted) unless list exceeds 30 jobs
 
-- As jobs run, AlbertJob objects are created automatically and stored in active_jobs.
+- As jobs run, OqtantJob objects are created automatically and stored in active_jobs.
 
   - View these jobs with see_active_jobs()
   - These jobs are available until the python session ends.
 
 - To operate on jobs from a current or previous session, load them into active_jobs with
 
   - load_job_from_id(), load_job_from_id_list(), load_job_from_file(), load_job_from_file_list()
 
-- To analyze job objects and use Albert's job analysis library, reference the AlbertJob class documentation.
+- To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.
 
 ## Considerations
 
-- Oqtant cannot interact with jobs that have been deleted via the Albert Web App
+- Oqtant cannot interact with jobs that have been deleted via the Oqtant Web App
 
 - Job results and limits are restricted to the account used to authenticate the Oqtant client
 
 - All jobs that have been submitted will be processed even if the Oqtant client session is ended before they complete
 
 ## Oqtant API
 
-The Oqtant API provides everything you need to get started working with AlbertJobs and the Albert REST API. For more information regarding the Albert REST API refer to our [Albert REST API Docs](albert_api_docs.md)
+The Oqtant API provides everything you need to get started working with OqtantJobs and the Oqtant REST API. For more information regarding the Oqtant REST API refer to our [Oqtant REST API Docs](albert_api_docs.md)
 
 ### get_user_token
 
-A utility function required for getting Oqtant authenticated with your Albert account. Starts up a server to handle the Auth0 authentication process and acquire a token. This helper function is located in `oqtant.util.auth`
+A utility function required for getting Oqtant authenticated with your Oqtant account. Starts up a server to handle the Auth0 authentication process and acquire a token. This helper function is located in `oqtant.util.auth`
 
 ```
 Returns:
     str: Auth0 user token
 ```
 
 ### get_oqtant_client
@@ -62,149 +62,149 @@
     token (str): the auth0 token required for interacting with the REST API
 Returns:
     OqtantClient: authenticated instance of OqtantClient
 ```
 
 ### get_job
 
-Gets an AlbertJob from the Albert REST API. This will always be a targeted query for a specific run. If the run is omitted then this will always return the first run of the job. Will return results for any job regardless of it's status. This function is a member of `OqtantClient`
+Gets an OqtantJob from the Oqtant REST API. This will always be a targeted query for a specific run. If the run is omitted then this will always return the first run of the job. Will return results for any job regardless of it's status. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_id (str): this is the external_id of the job to fetch
     run (int): the run to target, this defaults to the first run if omitted
 Returns:
-    AlbertJob: an AlbertJob instance with the values of the job queried
+    OqtantJob: an OqtantJob instance with the values of the job queried
 ```
 
 ### get_job_inputs_without_output
 
-Gets an AlbertJob from the Albert REST API. This can return all runs within a job or a single run based on whether a run value is provided. The AlbertJobs returned will be converted to dictionaries and will not have any output data, even if they are complete. This is useful for taking an existing job and creating a new one based on it's input data. This function is a member of `OqtantClient`
+Gets an OqtantJob from the Oqtant REST API. This can return all runs within a job or a single run based on whether a run value is provided. The OqtantJobs returned will be converted to dictionaries and will not have any output data, even if they are complete. This is useful for taking an existing job and creating a new one based on it's input data. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_id (str): this is the external_id of the job to fetch
     run (Union[int, None]): optional argument if caller wishes to only has a single run returned
-    include_notes (bool): optional argument if caller wishes to include any notes associated with AlbertJob inputs. Defaults to False is not provided
+    include_notes (bool): optional argument if caller wishes to include any notes associated with OqtantJob inputs. Defaults to False is not provided
 Returns:
-    Dict: a Dict representation of an AlbertJob instance
+    Dict: a Dict representation of an OqtantJob instance
 ```
 
 ### generate_albert_job
 
-Generates an instance of AlbertJob from the provided dictionary that contains the job details and input. Will validate the values and raise an informative error if any violations are found. This function is a member of `OqtantClient`
+Generates an instance of OqtantJob from the provided dictionary that contains the job details and input. Will validate the values and raise an informative error if any violations are found. This function is a member of `OqtantClient`
 
 ```
 Args:
     job (Dict): dictionary containing job details and input
 Returns:
-    AlbertJob: an AlbertJob instance containing the details and input from the provided dictionary
+    OqtantJob: an OqtantJob instance containing the details and input from the provided dictionary
 ```
 
 ### submit_job
 
-Submits a single AlbertJob to the Albert REST API. Upon successful submission this function will return a dictionary containing the external_id of the job and it's position in the queue. This function is a member of `OqtantClient`
+Submits a single OqtantJob to the Oqtant REST API. Upon successful submission this function will return a dictionary containing the external_id of the job and it's position in the queue. This function is a member of `OqtantClient`
 
 ```
 Args:
-    job (AlbertJob): the AlbertJob instance to submit for processing
+    job (OqtantJob): the OqtantJob instance to submit for processing
 Returns:
     Dict: dictionary containing the external_id of the job and it's queue position
 ```
 
 ### run_jobs
 
-Submits a list of AlbertJobs to the Albert REST API. This function provides some optional functionality to alter how it behaves. Providing it with an argument of track_status=True will make it wait and poll the Albert REST API until all jobs in the list have completed. The track_status functionality outputs each jobs current status as it is polling and opens up the ability to use the other optional arguments write and filename. The write and filename arguments enable the ability to have the results of each completed job written to a file. The value of filename is optional and if not provided will cause the files to be created using the external_id of each job. If running more than one job and using the filename argument it is required that the number of jobs in job_list match the number of values in filename. This function is a member of `OqtantClient`
+Submits a list of OqtantJobs to the Oqtant REST API. This function provides some optional functionality to alter how it behaves. Providing it with an argument of track_status=True will make it wait and poll the Oqtant REST API until all jobs in the list have completed. The track_status functionality outputs each jobs current status as it is polling and opens up the ability to use the other optional arguments write and filename. The write and filename arguments enable the ability to have the results of each completed job written to a file. The value of filename is optional and if not provided will cause the files to be created using the external_id of each job. If running more than one job and using the filename argument it is required that the number of jobs in job_list match the number of values in filename. This function is a member of `OqtantClient`
 
 ```
 Args:
-    job_list (List[AlbertJob]): the list of AlbertJob instances to submit for processing
+    job_list (List[OqtantJob]): the list of OqtantJob instances to submit for processing
     track_status (bool): optional argument to tell this function to either return immediately or wait and poll until all jobs have completed
     write (bool): optional argument to tell this function to write the results of each job to file when complete
     filename (Union[str, List[str]]): optional argument to be used in conjunction with the write argument. allows the caller to customize the name(s) of the files being created
 Returns:
     List[str]: list of the external_id(s) returned for each submitted job in job_list
 ```
 
 ### search_jobs
 
-Submits a query to the REST API to search for jobs that match the provided criteria. The search results will be limited to jobs that meet your Albert account access. This function is a member of `OqtantClient`
+Submits a query to the REST API to search for jobs that match the provided criteria. The search results will be limited to jobs that meet your Oqtant account access. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_type (JobSchema.JobType): the type of the jobs to search for
     name (JobSchema.JobName): the name of the job to search for
     submit_start (str): the earliest submit date of the jobs to search for
     submit_start (str): the latest submit date of the jobs to search for
     notes (str): the notes of the jobs to search for
 Returns:
     List[Dict]: a list of jobs matching the provided search criteria
 ```
 
 ### track_jobs
 
-Polls the Albert REST API with a list of job external_ids and waits until all of them have completed. Will output each job's status while it is polling and will output a message when all jobs have completed. This function provides some optional functionality to alter how it behaves. Providing it with an argument of write will have it write the results of each completed job to a file. There is an additional argument that can be used with write called filename. The value of filename is optional and if not provided will cause the files to be created using the external_id of each job. If tracking more than one job and using the filename argument it is required that the number of jobs in job_list match the number of values in filename. This function is a member of `OqtantClient`
+Polls the Oqtant REST API with a list of job external_ids and waits until all of them have completed. Will output each job's status while it is polling and will output a message when all jobs have completed. This function provides some optional functionality to alter how it behaves. Providing it with an argument of write will have it write the results of each completed job to a file. There is an additional argument that can be used with write called filename. The value of filename is optional and if not provided will cause the files to be created using the external_id of each job. If tracking more than one job and using the filename argument it is required that the number of jobs in job_list match the number of values in filename. This function is a member of `OqtantClient`
 
 ```
 Args:
     pending_jobs (List[str]): list of job external_ids to track
     write (bool): optional argument to tell this function to write the results of each job to file when complete
     filename (Union[str, List[str]]): optional argument to be used in conjunction with the write argument. allows the caller to customize the name(s) of the files being created
 ```
 
 ### load_job_from_id_list
 
-Loads AlbertJobs from the Albert REST API into the current active_jobs list using a list of job external_ids. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
+Loads OqtantJobs from the Oqtant REST API into the current active_jobs list using a list of job external_ids. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_id_list (List[str]): list of job external_ids to load
 ```
 
 ### load_job_from_id
 
-Loads an AlbertJob from the Albert REST API into the current active_jobs list using a job external_id. The results of the jobs loaded by this function can be targeted to a specific run if there are multiple. This function is a member of `OqtantClient`
+Loads an OqtantJob from the Oqtant REST API into the current active_jobs list using a job external_id. The results of the jobs loaded by this function can be targeted to a specific run if there are multiple. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_id (str): the external_id of the job to load
     run (int): optional argument to target a specific job run
 ```
 
 ### load_job_from_file_list
 
-Loads AlbertJobs from the Albert REST API into the current active_jobs list using a list of filenames containing AlbertJob info. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
+Loads OqtantJobs from the Oqtant REST API into the current active_jobs list using a list of filenames containing OqtantJob info. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
 
 ```
 Args:
-    file_list (List[str]): list of filenames containing AlbertJob information
+    file_list (List[str]): list of filenames containing OqtantJob information
 ```
 
 ### load_job_from_file
 
-Loads an AlbertJob from the Albert REST API into the current active_jobs list using a file containing AlbertJob info. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
+Loads an OqtantJob from the Oqtant REST API into the current active_jobs list using a file containing OqtantJob info. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
 
 ```
 Args:
-    file_list (List[str]): list of filenames containing AlbertJob information
+    file_list (List[str]): list of filenames containing OqtantJob information
 ```
 
 ### see_active_jobs
 
 Utility function to print out the current contents of the active_jobs list. The optional argument of refresh tells the function whether it should refresh the status of pending or running jobs before printing out the results. Refreshing also updates the data in active_jobs so if jobs were submitted but not tracked this is a way to check on their status. This function is a member of `OqtantClient`
 
 ```
 Args:
     refresh (bool): optional argument to refresh the data of jobs in active_jobs
 ```
 
 ### \_write_job_to_file
 
-Utility function to write an AlbertJob instance to a file. Requires the full filepath including the name of the file the write. Files that already exist will cannot be overwritten. This function is a member of `OqtantClient`
+Utility function to write an OqtantJob instance to a file. Requires the full filepath including the name of the file the write. Files that already exist will cannot be overwritten. This function is a member of `OqtantClient`
 
 ```
 Args:
-    job (AlbertJob): the AlbertJob instance to write to file
+    job (OqtantJob): the OqtantJob instance to write to file
     filepath (str): the full path to the file to write, including the name of the file
 ```
 
 <link href="main.css" rel="stylesheet" />
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_1_bec_jobs.ipynb` & `oqtant-0.14.4/documentation/tutorials/tutorial_1_bec_jobs.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974757263609255%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '### This walkthrough covers authorizing an Oqtant "*

 * *            'session using the Oqtant client, generating, running and viewing the results of a '*

 * *            "job. ###\\n')], delete: [2]}}, 1: {'source': {insert: [(0, '# Authenticate with "*

 * *            "Oqtant\\n'), (2, '## Before you can view and submit jobs you must first authenticate "*

 * *            "with your Oqtant account\\n')], delete: [2, 0]}}, 2: {'source': {insert: [(7, '    "*

 * *            "OqtantJob,\\n' […]*

```diff
@@ -3,27 +3,27 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Oqtant Tutorial 1: Getting Started #\n",
                 "\n",
-                "### This walkthrough covers authorizing an Albert session using the Oqtant client, generating, running and viewing the results of a job. ###\n",
+                "### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###\n",
                 "\n",
                 "For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Authenticate with Albert\n",
+                "# Authenticate with Oqtant\n",
                 "\n",
-                "## Before you can view and submit jobs you must first authenticate with your Albert account\n",
+                "## Before you can view and submit jobs you must first authenticate with your Oqtant account\n",
                 "\n",
                 "Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -33,15 +33,15 @@
                 "from matplotlib import pyplot as plt\n",
                 "from lmfit import Model\n",
                 "import numpy as np\n",
                 "import inspect\n",
                 "from oqtant.oqtant_client import get_oqtant_client\n",
                 "from oqtant.util.auth import get_user_token\n",
                 "from oqtant.schemas.job import (\n",
-                "    AlbertJob,\n",
+                "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
                 "    round_sig\n",
                 ")\n",
                 "\n",
                 "token = get_user_token()"
@@ -70,15 +70,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Generate parameters to create a job ##\n",
-                "Every Albert job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BEC job:"
+                "Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BEC job:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -112,15 +112,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Add notes to your job input (Optional) ##\n",
-                "Every Albert job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:"
+                "Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -131,17 +131,17 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Submit the job to run on the Albert hardware ##\n",
+                "## Submit the job to run on the Oqtant hardware ##\n",
                 "\n",
-                "**run_jobs(job_list=jobs)** takes a list of AlbertJob objects and submits them to the online queue for Albert Jobs. For each AlbertJob added to the queue a unique UUID is generated and associated to the job.\n",
+                "**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.\n",
                 "\n",
                 "The output of **run_jobs()** is a list of the unique UUIDs generated during submission. \n",
                 "\n",
                 "If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.\n",
                 "\n",
                 "If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:\n",
                 "\n",
@@ -188,23 +188,23 @@
                 "\n",
                 "The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. \n",
                 "\n",
                 "**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**. \n",
                 "\n",
                 "<span style=\"color:red\"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>\n",
                 "\n",
-                "To keep inputs and results organized, all jobs are handled as objects of the **AlbertJob** class. \n",
+                "To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class. \n",
                 "\n",
-                "<span style=\"color:red\"> Note: both BEC and BARRIER job types are represented as AlbertJob objects with different job_type fields </span>\n",
+                "<span style=\"color:red\"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>\n",
                 "\n",
-                "### To access information about a AlbertJob object ###\n",
+                "### To access information about a OqtantJob object ###\n",
                 "\n",
                 "**EXAMPLEJOB.DESIRED_INFO**\n",
                 "\n",
-                "AlbertJob objects have the following relevant fields:\n",
+                "OqtantJob objects have the following relevant fields:\n",
                 "\n",
                 " - name\n",
                 " - job_type\n",
                 " - status\n",
                 " - time_submit (datetime object)\n",
                 " - inputs list (see walkthrough 2 for specifics)\n",
                 "\n",
@@ -232,15 +232,15 @@
                 "If your job is in the PENDING or RUNNING state, wait for 1 minute and update/see active jobs again. When the job \"Example Ultracold Matter Generator Job\" shows status COMPLETE, proceed to the next code block\n",
                 "\n",
                 "\n",
                 "## Loading job results ##\n",
                 "\n",
                 "### From this session ###\n",
                 "\n",
-                "When a job is COMPLETE and the active jobs dictionary is updated, the AlbertJob object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary."
+                "When a job is COMPLETE and the active jobs dictionary is updated, the OqtantJob object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -252,15 +252,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Loading job results from a previous session ###\n",
                 "\n",
-                "When Albert is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs."
+                "When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -294,15 +294,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Viewing TOF images and slice plots ##\n",
                 "\n",
-                "The Albert system automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms. \n",
+                "The Oqtant system automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms. \n",
                 "\n",
                 "To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -328,15 +328,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Viewing atom cloud statistics ##\n",
                 "\n",
-                "The Albert system performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:"
+                "The Oqtant system performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -351,15 +351,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating jobs based off previous ones ##\n",
                 "\n",
-                "There may be times where you would like to create a new AlbertJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below."
+                "There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_1_bec_jobs.md` & `oqtant-0.14.4/documentation/tutorials/tutorial_1_bec_jobs.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Oqtant Tutorial 1: Getting Started
 
-### This walkthrough covers authorizing an Albert session using the Oqtant client, generating, running and viewing the results of a job.
+### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job.
 
 For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md
 
-# Authenticate with Albert
+# Authenticate with Oqtant
 
-## Before you can view and submit jobs you must first authenticate with your Albert account
+## Before you can view and submit jobs you must first authenticate with your Oqtant account
 
 Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
 
 ```python
 from matplotlib import pyplot as plt
 from lmfit import Model
 import numpy as np
 import inspect
 from oqtant.oqtant_client import get_oqtant_client
 from oqtant.util.auth import get_user_token
 from oqtant.schemas.job import (
-    AlbertJob,
+    OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
     round_sig
 )
 
 token = get_user_token()
@@ -37,15 +37,15 @@
 
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
 ## Generate parameters to create a job
 
-Every Albert job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BEC job:
+Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BEC job:
 
 ```python
 default_bec_job = {
     "name": "Example Ultracold Matter Generator Job",
     "job_type": "BEC",
     "inputs": [
         {
@@ -69,25 +69,25 @@
 
 example_bec_job = oqtant_client.generate_albert_job(job=default_bec_job)
 print(example_bec_job)
 ```
 
 ## Add notes to your job input (Optional)
 
-Every Albert job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
+Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
 
 ```python
 # In this example we are only working with a single input
 # so we will add the note to the first and only input in the array
 example_bec_job.inputs[0].notes = "This is an example BEC job created from Oqtant tutorial #1"
 ```
 
-## Submit the job to run on the Albert hardware
+## Submit the job to run on the Oqtant hardware
 
-**run_jobs(job_list=jobs)** takes a list of AlbertJob objects and submits them to the online queue for Albert Jobs. For each AlbertJob added to the queue a unique UUID is generated and associated to the job.
+**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.
 
 The output of **run_jobs()** is a list of the unique UUIDs generated during submission.
 
 If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.
 
 If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:
 
@@ -112,23 +112,23 @@
 
 The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session.
 
 **oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**.
 
 <span style="color:red"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>
 
-To keep inputs and results organized, all jobs are handled as objects of the **AlbertJob** class.
+To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class.
 
-<span style="color:red"> Note: both BEC and BARRIER job types are represented as AlbertJob objects with different job_type fields </span>
+<span style="color:red"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>
 
-### To access information about a AlbertJob object
+### To access information about a OqtantJob object
 
 **EXAMPLEJOB.DESIRED_INFO**
 
-AlbertJob objects have the following relevant fields:
+OqtantJob objects have the following relevant fields:
 
 - name
 - job_type
 - status
 - time_submit (datetime object)
 - inputs list (see walkthrough 2 for specifics)
 
@@ -144,24 +144,24 @@
 
 If your job is in the PENDING or RUNNING state, wait for 1 minute and update/see active jobs again. When the job "Example Ultracold Matter Generator Job" shows status COMPLETE, proceed to the next code block
 
 ## Loading job results
 
 ### From this session
 
-When a job is COMPLETE and the active jobs dictionary is updated, the AlbertJob object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary.
+When a job is COMPLETE and the active jobs dictionary is updated, the OqtantJob object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary.
 
 ```python
 example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]
 print(example_bec_job)
 ```
 
 ### Loading job results from a previous session
 
-When Albert is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs.
+When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs.
 
 ```python
 # for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run
 oqtant_client.load_job_from_id(example_bec_job_uuid)
 # access job from active_jobs
 example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]
 ```
@@ -173,15 +173,15 @@
 ```python
 for key in example_bec_job.inputs[0].output.values.dict().keys():
     print(key)
 ```
 
 ## Viewing TOF images and slice plots
 
-The Albert system automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms.
+The Oqtant system automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms.
 
 To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself.
 
 ```python
 example_bec_job.atoms_2dplot(figsize=(6,6))
 
 example_bec_job.atoms_sliceplot()
@@ -196,27 +196,27 @@
 plt.colorbar(TOF_plot, shrink=0.8)
 
 plt.show()
 ```
 
 ## Viewing atom cloud statistics
 
-The Albert system performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:
+The Oqtant system performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:
 
 ```python
 output = example_bec_job.inputs[0].output.values
 print("temperature (nK):"+ str(output.temperature_uk))
 print("total atoms :"+ str(output.tof_atom_number))
 print("condensed atoms :"+ str(output.condensed_atom_number))
 print("thermal atoms :"+ str(output.thermal_atom_number))
 ```
 
 ## Creating jobs based off previous ones
 
-There may be times where you would like to create a new AlbertJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below.
+There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below.
 
 ```python
 # identify the job you wish to copy, this can be any job id you want to use.
 # the status of the job does not matter
 already_submitted_job_id = example_bec_job.external_id
 
 # for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_2_barrier_jobs.ipynb` & `oqtant-0.14.4/documentation/tutorials/tutorial_2_barrier_jobs.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976974435866157%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '### This walkthrough covers authorizing an Oqtant "*

 * *            'session using the Oqtant client, generating, running and viewing the results of a '*

 * *            "job. ###\\n')], delete: [2]}}, 1: {'source': {insert: [(0, '# Authenticate with "*

 * *            "Oqtant\\n'), (2, '## Before you can view and submit jobs you must first authenticate "*

 * *            "with your Oqtant account\\n')], delete: [2, 0]}}, 2: {'source': {insert: [(7, '    "*

 * *            "OqtantJob,\\n' […]*

```diff
@@ -3,27 +3,27 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Oqtant Tutorial 2: Barrier Manipulator #\n",
                 "\n",
-                "### This walkthrough covers authorizing an Albert session using the Oqtant client, generating, running and viewing the results of a job. ###\n",
+                "### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###\n",
                 "\n",
                 "For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Authenticate with Albert\n",
+                "# Authenticate with Oqtant\n",
                 "\n",
-                "## Before you can view and submit jobs you must first authenticate with your Albert account\n",
+                "## Before you can view and submit jobs you must first authenticate with your Oqtant account\n",
                 "\n",
                 "Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -33,15 +33,15 @@
                 "from matplotlib import pyplot as plt\n",
                 "from lmfit import Model\n",
                 "import numpy as np\n",
                 "import inspect\n",
                 "from oqtant.oqtant_client import get_oqtant_client\n",
                 "from oqtant.util.auth import get_user_token\n",
                 "from oqtant.schemas.job import (\n",
-                "    AlbertJob,\n",
+                "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
                 "    round_sig\n",
                 ")\n",
                 "\n",
                 "token = get_user_token()"
@@ -70,15 +70,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Generate parameters to create a job ##\n",
-                "Every Albert job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BARRIER job:"
+                "Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BARRIER job:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -129,15 +129,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Add notes to your job input (Optional) ##\n",
-                "Every Albert job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:"
+                "Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -148,17 +148,17 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Submit the job to run on the Albert hardware ##\n",
+                "## Submit the job to run on the Oqtant hardware ##\n",
                 "\n",
-                "**run_jobs(job_list=jobs)** takes a list of AlbertJob objects and submits them to the online queue for Albert Jobs. For each AlbertJob added to the queue a unique UUID is generated and associated to the job.\n",
+                "**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.\n",
                 "\n",
                 "The output of **run_jobs()** is a list of the unique UUIDs generated during submission. \n",
                 "\n",
                 "If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.\n",
                 "\n",
                 "If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:\n",
                 "\n",
@@ -205,23 +205,23 @@
                 "\n",
                 "The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. \n",
                 "\n",
                 "**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**. \n",
                 "\n",
                 "<span style=\"color:red\"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>\n",
                 "\n",
-                "To keep inputs and results organized, all jobs are handled as objects of the **AlbertJob** class. \n",
+                "To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class. \n",
                 "\n",
-                "<span style=\"color:red\"> Note: both BEC and BARRIER job types are represented as AlbertJob objects with different job_type fields </span>\n",
+                "<span style=\"color:red\"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>\n",
                 "\n",
-                "### To access information about a AlbertJob object ###\n",
+                "### To access information about a OqtantJob object ###\n",
                 "\n",
                 "**EXAMPLEJOB.DESIRED_INFO**\n",
                 "\n",
-                "AlbertJob objects have the following relevant fields:\n",
+                "OqtantJob objects have the following relevant fields:\n",
                 "\n",
                 " - name\n",
                 " - job_type\n",
                 " - status\n",
                 " - time_submit (datetime object)\n",
                 " - inputs list (see walkthrough 2 for specifics)\n",
                 "\n",
@@ -264,15 +264,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Loading job results from a previous session ###\n",
                 "\n",
-                "When Albert is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs."
+                "When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -337,15 +337,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating jobs based off previous ones ##\n",
                 "\n",
-                "There may be times where you would like to create a new AlbertJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below."
+                "There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_2_barrier_jobs.md` & `oqtant-0.14.4/documentation/tutorials/tutorial_2_barrier_jobs.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Oqtant Tutorial 2: Barrier Manipulator
 
-### This walkthrough covers authorizing an Albert session using the Oqtant client, generating, running and viewing the results of a job.
+### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job.
 
 For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md
 
-# Authenticate with Albert
+# Authenticate with Oqtant
 
-## Before you can view and submit jobs you must first authenticate with your Albert account
+## Before you can view and submit jobs you must first authenticate with your Oqtant account
 
 Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook.
 
 ```python
 from matplotlib import pyplot as plt
 from lmfit import Model
 import numpy as np
 import inspect
 from oqtant.oqtant_client import get_oqtant_client
 from oqtant.util.auth import get_user_token
 from oqtant.schemas.job import (
-    AlbertJob,
+    OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
     round_sig
 )
 
 token = get_user_token()
@@ -37,15 +37,15 @@
 
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
 ## Generate parameters to create a job
 
-Every Albert job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BARRIER job:
+Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BARRIER job:
 
 ```python
 default_barrier_job = {
     "name": "Example Barrier Manipulator Job",
     "job_type": "BARRIER",
     "inputs": [
         {
@@ -86,25 +86,25 @@
 
 example_barrier_job = oqtant_client.generate_albert_job(job=default_barrier_job)
 print(example_barrier_job)
 ```
 
 ## Add notes to your job input (Optional)
 
-Every Albert job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
+Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
 
 ```python
 # In this example we are only working with a single input
 # so we will add the note to the first and only input in the array
 example_barrier_job.inputs[0].notes = "This is an example BARRIER job created from Oqtant tutorial #1"
 ```
 
-## Submit the job to run on the Albert hardware
+## Submit the job to run on the Oqtant hardware
 
-**run_jobs(job_list=jobs)** takes a list of AlbertJob objects and submits them to the online queue for Albert Jobs. For each AlbertJob added to the queue a unique UUID is generated and associated to the job.
+**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.
 
 The output of **run_jobs()** is a list of the unique UUIDs generated during submission.
 
 If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.
 
 If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:
 
@@ -129,23 +129,23 @@
 
 The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session.
 
 **oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**.
 
 <span style="color:red"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>
 
-To keep inputs and results organized, all jobs are handled as objects of the **AlbertJob** class.
+To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class.
 
-<span style="color:red"> Note: both BEC and BARRIER job types are represented as AlbertJob objects with different job_type fields </span>
+<span style="color:red"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>
 
-### To access information about a AlbertJob object
+### To access information about a OqtantJob object
 
 **EXAMPLEJOB.DESIRED_INFO**
 
-AlbertJob objects have the following relevant fields:
+OqtantJob objects have the following relevant fields:
 
 - name
 - job_type
 - status
 - time_submit (datetime object)
 - inputs list (see walkthrough 2 for specifics)
 
@@ -165,15 +165,15 @@
 
 ```python
 example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]
 ```
 
 ### Loading job results from a previous session
 
-When Albert is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs.
+When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs.
 
 ```python
 # for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run
 oqtant_client.load_job_from_id(example_barrier_job_uuid)
 # access job from active_jobs
 example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]
 ```
@@ -205,15 +205,15 @@
 plt.colorbar(IT_plot)
 
 plt.show()
 ```
 
 ## Creating jobs based off previous ones
 
-There may be times where you would like to create a new AlbertJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below.
+There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below.
 
 ```python
 # identify the job you wish to copy, this can be any job id you want to use.
 # the status of the job does not matter
 already_submitted_job_id = example_barrier_job.external_id
 
 # for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_3_abstractions.ipynb` & `oqtant-0.14.4/documentation/tutorials/tutorial_3_abstractions.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993714857266436%*

 * *Differences: {"'cells'": "{3: {'source': ['In this tutorial, we will explore the structure of jobs that you "*

 * *            'submit to Oqtant.  In an earlier tutorial, we saw that a basic BEC job could be '*

 * *            'defined by a dictionary structure like\']}, 5: {\'source\': {insert: [(0, "We could '*

 * *            "then feed the above data structure to the API's *generate_Oqtant_job()* function to "*

 * *            'create the job object.  Here, we would like to explore the contents of the underlying '*

 * *            'job data […]*

```diff
@@ -28,15 +28,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4942af2d",
             "metadata": {},
             "source": [
-                "In this tutorial, we will explore the structure of jobs that you submit to Albert.  In an earlier tutorial, we saw that a basic BEC job could be defined by a dictionary structure like"
+                "In this tutorial, we will explore the structure of jobs that you submit to Oqtant.  In an earlier tutorial, we saw that a basic BEC job could be defined by a dictionary structure like"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c08f5594",
             "metadata": {},
@@ -67,17 +67,17 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "61960d47",
             "metadata": {},
             "source": [
-                "We could then feed the above data structure to the API's *generate_Albert_job()* function to create the job object.  Here, we would like to explore the contents of the underlying job data structure more in depth.  The fields that control the behavior of the quantum matter machine are contained as *values* in the *inputs* list ([]).  For now, we will only discuss cases where the *inputs* list contains a single element.  When this list's length is greater than one, it signifies a so-called *batch* job, which will be discussed in a later tutorial.  \n",
+                "We could then feed the above data structure to the API's *generate_Oqtant_job()* function to create the job object.  Here, we would like to explore the contents of the underlying job data structure more in depth.  The fields that control the behavior of the quantum matter machine are contained as *values* in the *inputs* list ([]).  For now, we will only discuss cases where the *inputs* list contains a single element.  When this list's length is greater than one, it signifies a so-called *batch* job, which will be discussed in a later tutorial.  \n",
                 "\n",
-                "The contents of *values* includes directives on the type of imaging to perform (*image_type* etc.) and how long to run the experiment (*end_time_ms*) after evaporation to BEC is complete.  Also included are various job primitives that can be created and edited as programmable objects in their own right.  These primitives include *rf_evaporation*, *optical_barriers*, *optical_landscape*, and *lasers*.  Much like an *AlbertJob* itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object.  Although not shown explicitly in our simple job data structure above, both *optical_barriers* and *lasers* are lists containing *Barrier* and *Laser* objects, respectively.  These objects will be explored below.  You are likely already familiar with the structure of the *rf_evaporation* data and how defining that data controls the evaporation to BEC in the experiment.  The *optical_landscape* data is a bit more complicated and will be explored in more detail below in a dedicated section.       \n",
+                "The contents of *values* includes directives on the type of imaging to perform (*image_type* etc.) and how long to run the experiment (*end_time_ms*) after evaporation to BEC is complete.  Also included are various job primitives that can be created and edited as programmable objects in their own right.  These primitives include *rf_evaporation*, *optical_barriers*, *optical_landscape*, and *lasers*.  Much like an *OqtantJob* itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object.  Although not shown explicitly in our simple job data structure above, both *optical_barriers* and *lasers* are lists containing *Barrier* and *Laser* objects, respectively.  These objects will be explored below.  You are likely already familiar with the structure of the *rf_evaporation* data and how defining that data controls the evaporation to BEC in the experiment.  The *optical_landscape* data is a bit more complicated and will be explored in more detail below in a dedicated section.       \n",
                 "\n",
                 "Not all job types support every one of these data structures.  For the basic BEC-type job above, we did not have data entries for barriers, the landscape, or lasers.  BEC jobs, for instance, only support the rf_evaporation primitive.  After all, the purpose of a BEC job is to keep things simple and just focus on the ability to tune the creation of the condensate.  At the next level of complexity, BARRIER jobs support both *rf_evaporation* and *optical_barriers* but not \"optical_landscape\" or \"lasers\".  What data structures are supported by different job types will become clear as those job types are created/used/submitted.  As a preview, please refer to the following table.\n",
                 "\n",
                 "| Job type   | Supports       |                  |                   |        |\n",
                 "|------------|----------------|------------------|-------------------|--------|\n",
                 "|            | rf_evaporation | optical_barriers | optical_landscape | lasers |\n",
                 "| BEC        |                |                  |                   |        |\n",
@@ -115,15 +115,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d2a8885a",
             "metadata": {},
             "source": [
-                "Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific Albert job.  We can create this object by either calling the constructor directly with the required data fields:"
+                "Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific Oqtant job.  We can create this object by either calling the constructor directly with the required data fields:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8eecbfcf",
             "metadata": {},
@@ -540,15 +540,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "23affffd",
             "metadata": {},
             "source": [
-                "Another Albert job primitive is the (singular) 'OpticalLandscape' object.  This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment.  However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.    \n",
+                "Another Oqtant job primitive is the (singular) 'OpticalLandscape' object.  This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment.  However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.    \n",
                 "\n",
                 "The OpticalLandscape object consists of a list of individual potential-energy landscapes and an interpolation option on how those landscapes connect together *in time* (if there exists more than one underlying landscape).  Let us begin by constructing a couple Landscape objects, from which we will compose the OpticalLandscape container object.   "
             ]
         },
         {
             "cell_type": "markdown",
             "id": "758cae38",
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_3_abstractions.md` & `oqtant-0.14.4/documentation/tutorials/tutorial_3_abstractions.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ```python
 %matplotlib inline
 from bert_schemas import job as JobSchema
 ```
 
 ## Oqtant jobs and their constituent primitives
 
-In this tutorial, we will explore the structure of jobs that you submit to Albert. In an earlier tutorial, we saw that a basic BEC job could be defined by a dictionary structure like
+In this tutorial, we will explore the structure of jobs that you submit to Oqtant. In an earlier tutorial, we saw that a basic BEC job could be defined by a dictionary structure like
 
 ```python
 default_bec_job_data = {
     "name": "Example BEC Job",
     "job_type": "BEC",
     "inputs": [
         {
@@ -30,19 +30,19 @@
                 "lasers": None
             }
         }
     ]
 }
 ```
 
-We could then feed the above data structure to the API's _generate_Albert_job()_ function to create the job object. Here, we would like to explore the contents of the underlying job data structure more in depth. The fields that control the behavior of the quantum matter machine are contained as _values_ in the _inputs_ list ([]). For now, we will only discuss cases where the _inputs_ list contains a single element. When this list's length is greater than one, it signifies a so-called _batch_ job, which will be discussed in a later tutorial.
+We could then feed the above data structure to the API's _generate_Oqtant_job()_ function to create the job object. Here, we would like to explore the contents of the underlying job data structure more in depth. The fields that control the behavior of the quantum matter machine are contained as _values_ in the _inputs_ list ([]). For now, we will only discuss cases where the _inputs_ list contains a single element. When this list's length is greater than one, it signifies a so-called _batch_ job, which will be discussed in a later tutorial.
 
-The contents of _values_ includes directives on the type of imaging to perform (_image_type_ etc.) and how long to run the experiment (_end_time_ms_) after evaporation to BEC is complete. Also included are various job primitives that can be created and edited as programmable objects in their own right. These primitives include _rf_evaporation_, _optical_barriers_, _optical_landscape_, and _lasers_. Much like an _AlbertJob_ itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object. Although not shown explicitly in our simple job data structure above, both _optical_barriers_ and _lasers_ are lists containing _Barrier_ and _Laser_ objects, respectively. These objects will be explored below. You are likely already familiar with the structure of the _rf_evaporation_ data and how defining that data controls the evaporation to BEC in the experiment. The _optical_landscape_ data is a bit more complicated and will be explored in more detail below in a dedicated section.
+The contents of _values_ includes directives on the type of imaging to perform (_image_type_ etc.) and how long to run the experiment (_end_time_ms_) after evaporation to BEC is complete. Also included are various job primitives that can be created and edited as programmable objects in their own right. These primitives include _rf_evaporation_, _optical_barriers_, _optical_landscape_, and _lasers_. Much like an _OqtantJob_ itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object. Although not shown explicitly in our simple job data structure above, both _optical_barriers_ and _lasers_ are lists containing _Barrier_ and _Laser_ objects, respectively. These objects will be explored below. You are likely already familiar with the structure of the _rf_evaporation_ data and how defining that data controls the evaporation to BEC in the experiment. The _optical_landscape_ data is a bit more complicated and will be explored in more detail below in a dedicated section.
 
-Not all job types support every one of these data structures. For the basic BEC-type job above, we did not have data entries for barriers, the landscape, or lasers. BEC jobs, for instance, only support the rf_evaporation primitive. After all, the purpose of a BEC job is to keep things simple and just focus on the ability to tune the creation of the condensate. At the next level of complexity, BARRIER jobs support both _rf_evaporation_ and _optical_barriers_ but not "optical_landscape" or "lasers". What data structures are supported by different job types will become clear as those job types are created/used/submitted. As a preview, please refer to the following table.
+Not all job types support every one of these data structures. For the basic BEC-type job above, we did not have data entries for barriers, the landscape, or lasers. BEC jobs, for instance, only support the rf*evaporation primitive. After all, the purpose of a BEC job is to keep things simple and just focus on the ability to tune the creation of the condensate. At the next level of complexity, BARRIER jobs support both \_rf_evaporation* and _optical_barriers_ but not "optical_landscape" or "lasers". What data structures are supported by different job types will become clear as those job types are created/used/submitted. As a preview, please refer to the following table.
 
 | Job type   | Supports       |                  |                   |        |
 | ---------- | -------------- | ---------------- | ----------------- | ------ |
 |            | rf_evaporation | optical_barriers | optical_landscape | lasers |
 | BEC        |                |                  |                   |        |
 | BARRIER    | X              | X                |                   |        |
 | TRANSISTOR | X              | X                | X                 | X      |
@@ -54,15 +54,15 @@
 
 Every job input has exactly one constituent RfEvaporation object defined by the "rf_evaporation" data shown above. The behavior of this object controls the RF knife evaporation from an ultracold gas to Bose-Einstein condensate (BEC), as well as providing flexibility for applying RF fields during the experiment phase after the initial evaporation is complete. The evaporation stage results in a tradeoff between final atom number and temperature -- evaporating more deeply, signified by RF detuning values closer to 0, produces less atoms but at colder temperature (and correspondingly higher condensate fraction). Applying RF radiation during the experiment phase allows for hot atoms above some temperature, produced for example by rapid manipulation of optical barries or landscape potentials (explored below), to be removed the experiment -- a so-called "RF shield".
 
 It is important to note here that we adopt the convention that time = 0 refers to the _end_ of the evaporation period. As such, the initial evaporation to BEC, as defined by the object under current inspection, will involve negative (relative) times. In our trap, the entire evaporation cycle takes on the order of a second, and times are specified in ms, so we should see negative times as large as a few thousand ms.
 
 ### Construction
 
-Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific Albert job. We can create this object by either calling the constructor directly with the required data fields:
+Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific Oqtant job. We can create this object by either calling the constructor directly with the required data fields:
 
 ```python
 evap = JobSchema.RfEvaporation(
         times_ms = [-1600, -1200, -800, -400, 0],
         frequencies_mhz = [17.0, 8.0, 4.0, 1.2, 0.045],
         powers_mw = [500.0, 500.0, 475.0, 360.0, 220.0],
         interpolation = "LINEAR"
@@ -215,15 +215,15 @@
 barr.plot_potential(time = 5, x_limits = [-25,25])
 ```
 
 Note that the resolution of the projected light optical system is on the order of 2 microns. Thus, _Barrier_ objects with small widths will all appear similar in reality (the experiment) even if they have different _shape_ settings.
 
 ### Exploring Barrier interpolation options
 
-A Barrier object's 'interpolation' style determines how the time-dependent position, height, and width are determined for intermediate times between the provided data points in the 'times_ms' list class member. At this time, the interpolation choice is _shared_ for all three time-dependent barrier parameters. Let us explore the effects of different interpolation choices by altering the time-dependent position of our barrier, to make it a little more interesting, and then plot the position over time for a few different interpolation choices.
+A Barrier object's 'interpolation' style determines how the time-dependent position, height, and width are determined for intermediate times between the provided data points in the 'times*ms' list class member. At this time, the interpolation choice is \_shared* for all three time-dependent barrier parameters. Let us explore the effects of different interpolation choices by altering the time-dependent position of our barrier, to make it a little more interesting, and then plot the position over time for a few different interpolation choices.
 
 ```python
 barr.positions_um = [2, 4, 6, 8, 10, 2, 4, 6, 8, 6, 4]
 
 barr.interpolation = JobSchema.InterpolationType.STEP
 barr.plot_position()
 
@@ -235,15 +235,15 @@
 
 ```python
 print([e.value for e in JobSchema.InterpolationType])
 ```
 
 ## The Optical Landscape Object
 
-Another Albert job primitive is the (singular) 'OpticalLandscape' object. This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment. However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.
+Another Oqtant job primitive is the (singular) 'OpticalLandscape' object. This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment. However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.
 
 The OpticalLandscape object consists of a list of individual potential-energy landscapes and an interpolation option on how those landscapes connect together _in time_ (if there exists more than one underlying landscape). Let us begin by constructing a couple Landscape objects, from which we will compose the OpticalLandscape container object.
 
 ### Construction
 
 We can directly compose an _OpticalLandscape_ object, as above with the _Barrier_ object(s), or we can compose the constituent Landscape objects and then compose the full _OpticalLandscape_ object accordingly:
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_4_experiment.ipynb` & `oqtant-0.14.4/documentation/tutorials/tutorial_4_experiment.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985757550627907%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '### This walkthrough covers best practices for "*

 * *            'conducting experiments on the Oqtant system, including submitting batches of jobs, '*

 * *            "tracking experiment progress, and handling output data for later analysis. ###\\n')], "*

 * *            "delete: [2]}}, 1: {'source': {insert: [(0, '# Sign into Oqtant\\n'), (2, '## Before "*

 * *            "you can view and submit jobs you must first sign into your Oqtant account\\n')], "*

 * *            "delete: [2, 0 […]*

```diff
@@ -3,27 +3,27 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Oqtant Tutorial 3: BEC Experimentation #\n",
                 "\n",
-                "### This walkthrough covers best practices for conducting experiments on the Albert system, including submitting batches of jobs, tracking experiment progress, and handling output data for later analysis. ###\n",
+                "### This walkthrough covers best practices for conducting experiments on the Oqtant system, including submitting batches of jobs, tracking experiment progress, and handling output data for later analysis. ###\n",
                 "\n",
                 "For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Sign into Albert\n",
+                "# Sign into Oqtant\n",
                 "\n",
-                "## Before you can view and submit jobs you must first sign into your Albert account\n",
+                "## Before you can view and submit jobs you must first sign into your Oqtant account\n",
                 "\n",
                 "Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -35,15 +35,15 @@
                 "import numpy as np\n",
                 "import inspect\n",
                 "import copy\n",
                 "from oqtant.oqtant_client import get_oqtant_client\n",
                 "from oqtant.util.auth import get_user_token\n",
                 "from bert_schemas import job as JobSchema\n",
                 "from oqtant.schemas.job import (\n",
-                "    AlbertJob,\n",
+                "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
                 "    round_sig\n",
                 ")\n",
                 "import csv\n",
                 "\n",
@@ -103,15 +103,15 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Generate job parameters for the experiment with generate_albert_job ## \n",
                 "\n",
-                "This experiment consists of 3 job inputs and no repeated trials. Below is an example BEC job with default parameters, here we update the **rf_e_mhz** and **time_of_flight_ms** values for each input. Review the input parameters before submitting the experiment jobs to run on the Albert hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**"
+                "This experiment consists of 3 job inputs and no repeated trials. Below is an example BEC job with default parameters, here we update the **rf_e_mhz** and **time_of_flight_ms** values for each input. Review the input parameters before submitting the experiment jobs to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -180,15 +180,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "\n",
-                "## Accessing fields of AlbertJob, BecInput and BarrierInput objects ##\n",
+                "## Accessing fields of OqtantJob, BecInput and BarrierInput objects ##\n",
                 "\n",
                 "To access the above input parameters of a job object: \n",
                 "\n",
                 "**EXAMPLEJOB.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST**\n",
                 "\n",
                 "Here, we review the experiment parameters by accessing the \"input\" object which has the following fields:\n",
                 "\n",
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_4_experiment.md` & `oqtant-0.14.4/documentation/tutorials/tutorial_4_experiment.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Oqtant Tutorial 3: BEC Experimentation
 
-### This walkthrough covers best practices for conducting experiments on the Albert system, including submitting batches of jobs, tracking experiment progress, and handling output data for later analysis.
+### This walkthrough covers best practices for conducting experiments on the Oqtant system, including submitting batches of jobs, tracking experiment progress, and handling output data for later analysis.
 
 For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md
 
-# Sign into Albert
+# Sign into Oqtant
 
-## Before you can view and submit jobs you must first sign into your Albert account
+## Before you can view and submit jobs you must first sign into your Oqtant account
 
 Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook.
 
 ```python
 from matplotlib import pyplot as plt
 from lmfit import Model
 import numpy as np
 import inspect
 import copy
 from oqtant.oqtant_client import get_oqtant_client
 from oqtant.util.auth import get_user_token
 from bert_schemas import job as JobSchema
 from oqtant.schemas.job import (
-    AlbertJob,
+    OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
     round_sig
 )
 import csv
 
@@ -60,15 +60,15 @@
 ```python
 rf_e_values = [0.07, 0.03, 0.05]
 tof_interval_values = [10, 12, 15]
 ```
 
 ## Generate job parameters for the experiment with generate_albert_job
 
-This experiment consists of 3 job inputs and no repeated trials. Below is an example BEC job with default parameters, here we update the **rf_e_mhz** and **time_of_flight_ms** values for each input. Review the input parameters before submitting the experiment jobs to run on the Albert hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
+This experiment consists of 3 job inputs and no repeated trials. Below is an example BEC job with default parameters, here we update the **rf_e_mhz** and **time_of_flight_ms** values for each input. Review the input parameters before submitting the experiment jobs to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
 
 ```python
 experiment = {
     "name": "RF Sweep Experiment",
     "job_type": "BEC",
     "inputs": [
         {
@@ -125,15 +125,15 @@
     ],
 }
 
 experiment_job = oqtant_client.generate_albert_job(job=experiment)
 print(experiment_job)
 ```
 
-## Accessing fields of AlbertJob, BecInput and BarrierInput objects
+## Accessing fields of OqtantJob, BecInput and BarrierInput objects
 
 To access the above input parameters of a job object:
 
 **EXAMPLEJOB.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST**
 
 Here, we review the experiment parameters by accessing the "input" object which has the following fields:
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_5_optimization.ipynb` & `oqtant-0.14.4/documentation/tutorials/tutorial_5_optimization.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992182449903038%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '### This walkthrough reviews authorizing an Oqtant "*

 * *            "session and an example of optimization for BEC. ###\\n')], delete: [2]}}, 1: "*

 * *            "{'source': {insert: [(0, '# Sign into Oqtant\\n'), (2, '## Before you can view and "*

 * *            "submit jobs you must first sign into your Oqtant account\\n')], delete: [2, 0]}}, 2: "*

 * *            "{'source': {insert: [(14, '    OqtantJob,\\n')], delete: [14]}}, 24: {'source': "*

 * *            "{insert: [(2, '#Oq […]*

```diff
@@ -3,27 +3,27 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Oqtant Tutorial 4: BEC Experimentation #\n",
                 "\n",
-                "### This walkthrough reviews authorizing an Albert session and an example of optimization for BEC. ###\n",
+                "### This walkthrough reviews authorizing an Oqtant session and an example of optimization for BEC. ###\n",
                 "\n",
                 "For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Sign into Albert\n",
+                "# Sign into Oqtant\n",
                 "\n",
-                "## Before you can view and submit jobs you must first sign into your Albert account\n",
+                "## Before you can view and submit jobs you must first sign into your Oqtant account\n",
                 "\n",
                 "Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -40,15 +40,15 @@
                 "import numpy as np\n",
                 "import inspect\n",
                 "import copy\n",
                 "from oqtant.oqtant_client import get_oqtant_client\n",
                 "from oqtant.util.auth import get_user_token\n",
                 "from bert_schemas import job as JobSchema\n",
                 "from oqtant.schemas.job import (\n",
-                "    AlbertJob,\n",
+                "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
                 "    round_sig\n",
                 ")\n",
                 "import csv\n",
                 "\n",
@@ -423,39 +423,39 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#X = sample_domain\n",
                 "#y = np.asarray([cost_func_9D(x) for x in X])\n",
-                "#Albert_model = GPR()\n",
-                "#Albert_model.fit(X, y)\n",
+                "#Oqtant_model = GPR()\n",
+                "#Oqtant_model.fit(X, y)\n",
                 "\n",
                 "X = X_global_train\n",
                 "y = y_global_train\n",
-                "Albert_model = GPR()\n",
-                "Albert_model.fit(X_global_train, y_global_train)\n",
+                "Oqtant_model = GPR()\n",
+                "Oqtant_model.fit(X_global_train, y_global_train)\n",
                 "\n",
                 "cost = []\n",
                 "\n",
                 "for i in range(20):\n",
                 "    # select the next point to sample\n",
-                "    x = optimize_acquisition(X, y, Albert_model, 500)\n",
+                "    x = optimize_acquisition(X, y, Oqtant_model, 500)\n",
                 "    print('x', x)\n",
                 "    # sample the point\n",
                 "    actual = cost_func_9D(x)\n",
                 "    cost.append(actual)\n",
                 "    # summarize the finding\n",
-                "    est, _ = surrogate(Albert_model, [x])\n",
+                "    est, _ = surrogate(Oqtant_model, [x])\n",
                 "    print(x, est, actual)\n",
                 "    # add the data to the dataset\n",
                 "    X = np.vstack((X, [x]))\n",
                 "    y.append(actual)\n",
                 "    # update the model\n",
-                "    Albert_model.fit(X, y)"
+                "    Oqtant_model.fit(X, y)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `oqtant-0.14.2/documentation/tutorials/tutorial_5_optimization.md` & `oqtant-0.14.4/documentation/tutorials/tutorial_5_optimization.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Oqtant Tutorial 4: BEC Experimentation
 
-### This walkthrough reviews authorizing an Albert session and an example of optimization for BEC.
+### This walkthrough reviews authorizing an Oqtant session and an example of optimization for BEC.
 
 For more information about Oqtant refer to our documentation: https://albert-dev.coldquanta.com/oqtant/manual.md
 
-# Sign into Albert
+# Sign into Oqtant
 
-## Before you can view and submit jobs you must first sign into your Albert account
+## Before you can view and submit jobs you must first sign into your Oqtant account
 
 Run the below cell to be re-directed to our login page and provide you account credentials. Once authenticated you can safely close out that tab and return to this notebook.
 
 ```python
 from sklearn.gaussian_process import GaussianProcessRegressor as GPR
 from matplotlib import pyplot as plt
 from scipy.optimize import minimize
@@ -21,15 +21,15 @@
 import numpy as np
 import inspect
 import copy
 from oqtant.oqtant_client import get_oqtant_client
 from oqtant.util.auth import get_user_token
 from bert_schemas import job as JobSchema
 from oqtant.schemas.job import (
-    AlbertJob,
+    OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
     round_sig
 )
 import csv
 
@@ -286,39 +286,39 @@
 ```
 
 ## Perform the optimization
 
 ```python
 #X = sample_domain
 #y = np.asarray([cost_func_9D(x) for x in X])
-#Albert_model = GPR()
-#Albert_model.fit(X, y)
+#Oqtant_model = GPR()
+#Oqtant_model.fit(X, y)
 
 X = X_global_train
 y = y_global_train
-Albert_model = GPR()
-Albert_model.fit(X_global_train, y_global_train)
+Oqtant_model = GPR()
+Oqtant_model.fit(X_global_train, y_global_train)
 
 cost = []
 
 for i in range(20):
     # select the next point to sample
-    x = optimize_acquisition(X, y, Albert_model, 500)
+    x = optimize_acquisition(X, y, Oqtant_model, 500)
     print('x', x)
     # sample the point
     actual = cost_func_9D(x)
     cost.append(actual)
     # summarize the finding
-    est, _ = surrogate(Albert_model, [x])
+    est, _ = surrogate(Oqtant_model, [x])
     print(x, est, actual)
     # add the data to the dataset
     X = np.vstack((X, [x]))
     y.append(actual)
     # update the model
-    Albert_model.fit(X, y)
+    Oqtant_model.fit(X, y)
 ```
 
 ```python
 # plot all samples and the final surrogate function
 plt.plot(cost[5:])
 #plt.yscale("log")
 plt.xlabel("function evaluations")
```

### Comparing `oqtant-0.14.2/oqtant/oqtant_client.py` & `oqtant-0.14.4/oqtant/oqtant_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,47 +7,47 @@
 
 import jwt
 import requests
 import semver
 from bert_schemas import job as job_schema
 from pydantic import ValidationError
 
-from oqtant.schemas.job import AlbertJob
+from oqtant.schemas.job import OqtantJob
 from oqtant.settings import Settings
 from oqtant.util import exceptions as api_exceptions
 
 settings = Settings()
 
 
 class OqtantClient:
-    """Python class for interacting with Albert
+    """Python class for interacting with Oqtant
     This class contains tools for:
-        - Accessing all of the functionality of the Albert Web App (https://albert-dev.coldquanta.com)
+        - Accessing all of the functionality of the Oqtant Web App (https://albert-dev.coldquanta.com)
             - BARRIER (Barrier Manipulator) jobs
             - BEC (Ultracold Matter) jobs
-        - Building parameterized (i.e. optimization) experiments using AlbertJobs
-        - Submitting and retrieving AlbertJob results
+        - Building parameterized (i.e. optimization) experiments using OqtantJobs
+        - Submitting and retrieving OqtantJob results
     How Oqtant works:
-        1.) Construct a single or list of AlbertJobs using 'generate_albert_job()'
-        2.) Run the single or list of AlbertJobs on the Albert hardware using 'run_jobs()'
-            - There is a limit of 30 AlbertJobs per use of 'run_jobs()'
-        3.) As AlbertJobs are running, the results are automatically stored in 'active_jobs'
-            - The AlbertJobs stored in 'active_jobs' are available until the python session ends
-        4.) If you choose to not track the status of AlbertJobs with 'run_jobs()' you can see the status
-            of your session's active AlbertJobs with 'see_active_jobs()'
+        1.) Construct a single or list of OqtantJobs using 'generate_albert_job()'
+        2.) Run the single or list of OqtantJobs on the Oqtant hardware using 'run_jobs()'
+            - There is a limit of 30 OqtantJobs per use of 'run_jobs()'
+        3.) As OqtantJobs are running, the results are automatically stored in 'active_jobs'
+            - The OqtantJobs stored in 'active_jobs' are available until the python session ends
+        4.) If you choose to not track the status of OqtantJobs with 'run_jobs()' you can see the status
+            of your session's active OqtantJobs with 'see_active_jobs()'
         5.) To operate on jobs submitted in a previous session you can load them into your 'active_jobs'
             by using either 'load_job_from_id()' or 'load_job_from_file()'
-        6.) To analyze AlbertJob objects and use Albert's job analysis library reference the AlbertJob
+        6.) To analyze OqtantJob objects and use Oqtant's job analysis library reference the OqtantJob
             class documentation located in 'oqtant/job.py'
     Need help? Found a bug? Contact albert@infleqtion.com for support. Thank you!
     """
 
     def __init__(self, *, settings, token, debug: bool = False):
         self.base_url: str = settings.base_url
-        self.active_jobs: dict[str, AlbertJob] = {}
+        self.active_jobs: dict[str, OqtantJob] = {}
         self.token: str = token
         self.max_ind_var: int = settings.max_ind_var
         self.max_job_batch_size: int = settings.max_job_batch_size
         self.debug: bool = debug
         self.version = version("oqtant")
 
         if not self.debug:
@@ -59,57 +59,57 @@
             dict: a dict of header information
         """
         return {
             "Authorization": f"Bearer {self.token}",
             "X-Client-Version": version("oqtant"),
         }
 
-    def get_job(self, job_id: str, run: int = 1) -> AlbertJob:
-        """Gets an AlbertJob from the Albert REST API. This will always be a targeted query
+    def get_job(self, job_id: str, run: int = 1) -> OqtantJob:
+        """Gets an OqtantJob from the Oqtant REST API. This will always be a targeted query
            for a specific run. If the run is omitted then this will always return the first
            run of the job. Will return results for any job regardless of it's status.
         Args:
             job_id (str): this is the external_id of the job to fetch
             run (int): the run to target, this defaults to the first run if omitted
         Returns:
-            AlbertJob: an AlbertJob instance with the values of the job queried
+            OqtantJob: an OqtantJob instance with the values of the job queried
         """
         request_url = f"{self.base_url}/{job_id}"
         params = {"run": run}
         response = requests.get(
             url=request_url,
             params=params,
             headers=self.__get_headers(),
             timeout=(5, 30),
         )
         if response.status_code in [401, 403]:
             raise api_exceptions.AuthorizationError
         response.raise_for_status()
         job_data = response.json()
         try:
-            job = AlbertJob(**job_data)
+            job = OqtantJob(**job_data)
         except (KeyError, ValidationError) as err:
             raise api_exceptions.ValidationError(f"Failed to get job {job_id}: {err}")
         return job
 
     def get_job_inputs_without_output(
         self, job_id: str, run: int | None = None, include_notes: bool = False
     ) -> dict:
-        """Gets an AlbertJob from the Albert REST API. This can return all runs within a job
-           or a single run based on whether a run value is provided. The AlbertJobs returned
+        """Gets an OqtantJob from the Oqtant REST API. This can return all runs within a job
+           or a single run based on whether a run value is provided. The OqtantJobs returned
            will be converted to dictionaries and will not have any output data, even if
            they are complete. This is useful for taking an existing job and creating a new one
            based on it's input data.
         Args:
            job_id (str): this is the external_id of the job to fetch
            run (Union[int, None]): optional argument if caller wishes to only has a single run returned
            include_notes (bool): optional argument if caller wishes to include any notes associated
-              with AlbertJob inputs. Defaults to False is not provided
+              with OqtantJob inputs. Defaults to False is not provided
         Returns:
-           dict: a dict representation of an AlbertJob instance
+           dict: a dict representation of an OqtantJob instance
         """
         request_url = f"{self.base_url}/{job_id}"
         params = {"exclude_input_output": True}
         if run:
             params["run"] = run
         response = requests.get(
             url=request_url,
@@ -118,51 +118,51 @@
             timeout=(5, 30),
         )
         if response.status_code in [401, 403]:
             raise api_exceptions.AuthorizationError
         response.raise_for_status()
         job_data = response.json()
         try:
-            job = AlbertJob(**job_data)
+            job = OqtantJob(**job_data)
         except (KeyError, ValidationError) as err:
             raise api_exceptions.ValidationError(f"Failed to get job {job_id}: {err}")
         if not include_notes:
             job.inputs[0].notes = ""
         job = job.dict()
         job.pop("input_count")
         return job
 
-    def generate_albert_job(self, *, job: dict) -> AlbertJob:
-        """Generates an instance of AlbertJob from the provided dictionary that contains the
+    def generate_albert_job(self, *, job: dict) -> OqtantJob:
+        """Generates an instance of OqtantJob from the provided dictionary that contains the
            job details and input. Will validate the values and raise an informative error if
            any violations are found.
         Args:
            job (dict): dictionary containing job details and input
         Returns:
-           AlbertJob: an AlbertJob instance containing the details and input from the provided
+           OqtantJob: an OqtantJob instance containing the details and input from the provided
               dictionary
         """
         try:
-            albert_job = AlbertJob(**job)
+            albert_job = OqtantJob(**job)
         except ValidationError as err:
-            raise api_exceptions.ValidationError(f"Failed to generate AlbertJob: {err}")
+            raise api_exceptions.ValidationError(f"Failed to generate OqtantJob: {err}")
         return albert_job
 
-    def submit_job(self, *, job: AlbertJob) -> dict:
-        """Submits a single AlbertJob to the Albert REST API. Upon successful submission this
+    def submit_job(self, *, job: OqtantJob) -> dict:
+        """Submits a single OqtantJob to the Oqtant REST API. Upon successful submission this
            function will return a dictionary containing the external_id of the job and it's
            position in the queue.
         Args:
-           job (AlbertJob): the AlbertJob instance to submit for processing
+           job (OqtantJob): the OqtantJob instance to submit for processing
         Returns:
            dict: dictionary containing the external_id of the job and it's queue position
         """
-        if not isinstance(job, AlbertJob):
+        if not isinstance(job, OqtantJob):
             try:
-                job = AlbertJob(**job)
+                job = OqtantJob(**job)
             except (TypeError, AttributeError, ValidationError) as err:
                 raise api_exceptions.ValidationError(f"Job is invalid: {err}")
         data = {
             "name": job.name,
             "job_type": job.job_type,
             "input_count": len(job.inputs),
             "inputs": [input.dict() for input in job.inputs],
@@ -177,32 +177,32 @@
             raise api_exceptions.AuthorizationError
         response.raise_for_status()
         response_data = response.json()
         return response_data
 
     def run_jobs(
         self,
-        job_list: list[AlbertJob],
+        job_list: list[OqtantJob],
         track_status: bool = False,
         write: bool = False,
         filename: str | list[str] = "",
     ) -> list[str]:
-        """Submits a list of AlbertJobs to the Albert REST API. This function provides some
+        """Submits a list of OqtantJobs to the Oqtant REST API. This function provides some
            optional functionality to alter how it behaves. Providing it with an argument of
-           track_status=True will make it wait and poll the Albert REST API until all jobs
+           track_status=True will make it wait and poll the Oqtant REST API until all jobs
            in the list have completed. The track_status functionality outputs each jobs
            current status as it is polling and opens up the ability to use the other optional
            arguments write and filename. The write and filename arguments enable the ability
            to have the results of each completed job written to a file. The value of filename
            is optional and if not provided will cause the files to be created using the
            external_id of each job. If running more than one job and using the filename
            argument it is required that the number of jobs in job_list match the number of
            values in filename.
         Args:
-           job_list (list[AlbertJob]): the list of AlbertJob instances to submit for processing
+           job_list (list[OqtantJob]): the list of OqtantJob instances to submit for processing
            track_status (bool): optional argument to tell this function to either return
              immediately or wait and poll until all jobs have completed
            write (bool): optional argument to tell this function to write the results of each
              job to file when complete
            filename (Union[str, list[str]]): optional argument to be used in conjunction with the
              write argument. allows the caller to customize the name(s) of the files being created
         Returns:
@@ -240,15 +240,15 @@
         job_type: job_schema.JobType | None = None,
         name: job_schema.JobName | None = None,
         submit_start: str | None = None,
         submit_end: str | None = None,
         notes: str | None = None,
     ) -> list[dict]:
         """Submits a query to the REST API to search for jobs that match the provided criteria.
-           The search results will be limited to jobs that meet your Albert account access.
+           The search results will be limited to jobs that meet your Oqtant account access.
         Args:
            job_type (job_schema.JobType): the type of the jobs to search for
            name (job_schema.JobName): the name of the job to search for
            submit_start (str): the earliest submit date of the jobs to search for
            submit_start (str): the latest submit date of the jobs to search for
            notes (str): the notes of the jobs to search for
         Returns:
@@ -275,15 +275,15 @@
     def track_jobs(
         self,
         *,
         pending_jobs: list[str],
         filename: str | list = "",
         write: bool = False,
     ) -> None:
-        """Polls the Albert REST API with a list of job external_ids and waits until all of them have
+        """Polls the Oqtant REST API with a list of job external_ids and waits until all of them have
            completed. Will output each job's status while it is polling and will output a message when
            all jobs have completed. This function provides some optional functionality to alter how it
            behaves. Providing it with an argument of write will have it write the results of each
            completed job to a file. There is an additional argument that can be used with write called
            filename. The value of filename is optional and if not provided will cause the files to be
            created using the external_id of each job. If tracking more than one job and using the
            filename argument it is required that the number of jobs in job_list match the number of
@@ -329,25 +329,25 @@
                     pending_jobs.remove(pending_job)
                     if write:
                         job_filenames.pop(0)
                 time.sleep(2)
         print("all jobs complete")
 
     def load_job_from_id_list(self, job_id_list: list[str]) -> None:
-        """Loads AlbertJobs from the Albert REST API into the current active_jobs list using a list
+        """Loads OqtantJobs from the Oqtant REST API into the current active_jobs list using a list
            of job external_ids. The results of the jobs loaded by this function are limited to their
            first run.
         Args:
            job_id_list (list[str]): list of job external_ids to load
         """
         for job_id in job_id_list:
             self.load_job_from_id(job_id)
 
     def load_job_from_id(self, job_id: str, run: int = 1) -> None:
-        """Loads an AlbertJob from the Albert REST API into the current active_jobs list using a job
+        """Loads an OqtantJob from the Oqtant REST API into the current active_jobs list using a job
            external_id. The results of the jobs loaded by this function can be targeted to a specific
            run if there are multiple.
         Args:
            job_id (str): the external_id of the job to load
            run (int): optional argument to target a specific job run
         """
         try:
@@ -356,29 +356,29 @@
             print(f"Loaded job: {job.name} {job_id}")
         except Exception as err:
             raise api_exceptions.ValidationError(
                 f"Failed to fetch job {job_id}: {err}. Please contact ColdQuanta if error persists"
             )
 
     def load_job_from_file_list(self, file_list: list[str]) -> None:
-        """Loads AlbertJobs from the Albert REST API into the current active_jobs list using a list
-           of filenames containing AlbertJob info. The results of the jobs loaded by this function are
+        """Loads OqtantJobs from the Oqtant REST API into the current active_jobs list using a list
+           of filenames containing OqtantJob info. The results of the jobs loaded by this function are
            limited to their first run.
         Args:
-           file_list (list[str]): list of filenames containing AlbertJob information
+           file_list (list[str]): list of filenames containing OqtantJob information
         """
         for f in file_list:
             self.load_job_from_file(f)
 
     def load_job_from_file(self, file: str) -> None:
-        """Loads an AlbertJob from the Albert REST API into the current active_jobs list using a file
-           containing AlbertJob info. The results of the jobs loaded by this function are limited to
+        """Loads an OqtantJob from the Oqtant REST API into the current active_jobs list using a file
+           containing OqtantJob info. The results of the jobs loaded by this function are limited to
            their first run.
         Args:
-           file_list (list[str]): list of filenames containing AlbertJob information
+           file_list (list[str]): list of filenames containing OqtantJob information
         """
         try:
             with open(file) as json_file:
                 data = json.load(json_file)
                 self.load_job_from_id(data["external_id"])
         except (FileNotFoundError, Exception) as err:
             raise api_exceptions.JobReadError(f"Failed to load job from {file}: {err}")
@@ -404,20 +404,20 @@
                     self.active_jobs[external_id] = refreshed_job
         print("ACTIVE JOBS")
         print("NAME\t\tSTATUS\t\tTIME SUBMIT\t\tID")
         print("_" * 50)
         for job_id, job in self.active_jobs.items():
             print(f"{job.name}\t\t{job.status}\t\t{job.time_submit}\t\t{job_id}")
 
-    def _write_job_to_file(self, job: AlbertJob, filepath: str) -> None:
-        """Utility function to write an AlbertJob instance to a file. Requires the full filepath
+    def _write_job_to_file(self, job: OqtantJob, filepath: str) -> None:
+        """Utility function to write an OqtantJob instance to a file. Requires the full filepath
            including the name of the file the write. Files that already exist cannot be
            overwritten.
         Args:
-           job (AlbertJob): the AlbertJob instance to write to file
+           job (OqtantJob): the OqtantJob instance to write to file
            filepath (str): the full path to the file to write, including the name of the file
         """
         if os.path.exists(filepath):
             raise api_exceptions.JobWriteError(
                 "File already exists. Please choose a unique filename."
             )
```

### Comparing `oqtant-0.14.2/oqtant/schemas/job.py` & `oqtant-0.14.4/oqtant/schemas/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     """
 
     return Gaussian_dist_2D(xy_mesh, GpOD, xc, yc, sigx, sigy, os) + TF_dist_2D(
         xy_mesh, TFpOD, xc, yc, rx, ry, os
     )
 
 
-class AlbertJob(job_schema.JobCreate):
+class OqtantJob(job_schema.JobCreate):
     external_id: UUID | None
     time_submit: datetime | None
     pix_cal: float = Field(8.71, const=True)
     sig_abs: float = Field(0.297, const=True)
     omega_x: float = Field(OMEGA_X, const=True)
     omega_y: float = Field(OMEGA_Y, const=True)
```

### Comparing `oqtant-0.14.2/oqtant/settings.py` & `oqtant-0.14.4/oqtant/settings.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.2/oqtant/util/auth.py` & `oqtant-0.14.4/oqtant/util/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     resp = requests.post(
         url, headers=headers, data=data, allow_redirects=False, timeout=(5, 30)
     )
     return resp.json()
 
 
 def get_user_token() -> str:
-    """A utility function required for getting Oqtant authenticated with your Albert account.
+    """A utility function required for getting Oqtant authenticated with your Oqtant account.
        Starts up a server to handle the Auth0 authentication process and acquire a token.
     Returns:
         str: Auth0 user token
     """
     server_config = uvicorn.Config(
         app=app, host="localhost", port=8080, log_level="error"
     )
```

### Comparing `oqtant-0.14.2/oqtant/util/exceptions.py` & `oqtant-0.14.4/oqtant/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.2/pyproject.toml` & `oqtant-0.14.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oqtant"
-version = "0.14.2"
+version = "0.14.4"
 description = "Oqtant Desktop Suite"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Hannah North <hannah.north@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
@@ -34,17 +34,18 @@
 urllib3 = "^1.26.12"
 notebook = "^6.4.12"
 lmfit = "^1.0.3"
 fastapi = "^0.92.0"
 uvicorn = { extras = ["standard"], version = "^0.20.0" }
 scikit-learn = "^1.2.0"
 python-dotenv = "^0.21.1"
-bert-schemas = "^1.17.0"
+bert-schemas = "^1.18.0"
 pyjwt = { extras = ["crypto"], version = "^2.6.0" }
 semver = "^3.0.0"
+ipykernel = "^6.23.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-xdist = "^3.2.0"
 pytest-ordering = "^0.6"
 pytest-cov = "^4.0.0"
 pycodestyle = "^2.10.0"
```

### Comparing `oqtant-0.14.2/PKG-INFO` & `oqtant-0.14.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: oqtant
-Version: 0.14.2
+Version: 0.14.4
 Summary: Oqtant Desktop Suite
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: bert-schemas (>=1.17.0,<2.0.0)
+Requires-Dist: bert-schemas (>=1.18.0,<2.0.0)
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
+Requires-Dist: ipykernel (>=6.23.1,<7.0.0)
 Requires-Dist: lmfit (>=1.0.3,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.2,<3.7.0)
 Requires-Dist: notebook (>=6.4.12,<7.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: pydantic (>=1.10.1,<2.0.0)
 Requires-Dist: pyjwt[crypto] (>=2.6.0,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
@@ -43,47 +44,47 @@
 pip install oqtant
 ```
 
 ## 🧭 Introduction
 
 This API contains tools to:
 
-- Access all the functionality of the Albert Web App (https://albert.coldquanta.com)
+- Access all the functionality of the Albert Web App (https://albert-dev.coldquanta.com)
 
   - BARRIER (Barrier Manipulator) jobs
   - BEC (Ultracold Matter) jobs
 
-- Build parameterized (i.e. optimization) experiments using AlbertJobs
+- Build parameterized (i.e. optimization) experiments using OqtantJobs
 
-- Submit and retrieve AlbertJob results
+- Submit and retrieve OqtantJob results
 
 ## 🤖 How Oqtant Works
 
-- Construct a single or list of jobs using the AlbertJob class
+- Construct a single or list of jobs using the OqtantJob class
 
   - 1D parameter sweeps are supported
 
 - Run a single or list of jobs using run_jobs(). The jobs are submitted to run on hardware in FIFO queue.
 
   - job lists are run sequentially (uninterrupted) unless list exceeds 30 jobs
 
-- As jobs run, AlbertJob objects are created automatically and stored in active_jobs.
+- As jobs run, OqtantJob objects are created automatically and stored in active_jobs.
 
   - View these jobs with see_active_jobs()
   - These jobs are available until the python session ends.
 
 - To operate on jobs from a current or previous session, load them into active_jobs with
 
   - load_job_from_id(), load_job_from_id_list(), load_job_from_file(), load_job_from_file_list()
 
-- To analyze job objects and use Albert's job analysis library, reference the AlbertJob class documentation.
+- To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.
 
 Need help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!
 
 ## 📓 Documentation
 
-- [Getting started](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/INSTALL.md) (installation, setting up the environment, How to run the tutorial notebooks)
-- [Tutorials](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/tutorials/tutorials.md) (demos for creating and submitting jobs)
-- [Oqtant API docs](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/oqtant_api_docs.md)
-- [Albert API docs](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/albert_api_docs.md)
-- [Job Analysis docs](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/job_analysis_docs.md)
+- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, How to run the tutorial notebooks)
+- [Tutorials](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/tutorials/tutorials.md) (demos for creating and submitting jobs)
+- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oqtant_api_docs.md)
+- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/albert_api_docs.md)
+- [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)
```


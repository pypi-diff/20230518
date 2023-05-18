# Comparing `tmp/seeq-spy-187.2.tar.gz` & `tmp/seeq-spy-187.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeq-spy-187.2.tar", last modified: Tue May  2 20:22:00 2023, max compression
+gzip compressed data, was "seeq-spy-187.5.tar", last modified: Wed May 17 17:45:36 2023, max compression
```

## Comparing `seeq-spy-187.2.tar` & `seeq-spy-187.5.tar`

### file list

```diff
@@ -1,149 +1,151 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.247388 seeq-spy-187.2/
--rw-rw-rw-   0        0        0    33551 2023-03-28 23:18:24.000000 seeq-spy-187.2/LICENSE
--rw-rw-rw-   0        0        0      207 2023-03-28 23:18:24.000000 seeq-spy-187.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4606 2023-05-02 20:22:00.246389 seeq-spy-187.2/PKG-INFO
--rw-rw-rw-   0        0        0     4091 2023-04-18 22:49:07.000000 seeq-spy-187.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.020390 seeq-spy-187.2/seeq/
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.038389 seeq-spy-187.2/seeq/base/
--rw-rw-rw-   0        0        0       36 2023-05-02 20:21:55.000000 seeq-spy-187.2/seeq/base/__init__.py
--rw-rw-rw-   0        0        0      875 2023-05-02 20:21:55.000000 seeq-spy-187.2/seeq/base/proputil.py
--rw-rw-rw-   0        0        0    31907 2023-05-02 20:21:55.000000 seeq-spy-187.2/seeq/base/seeq_names.py
--rw-rw-rw-   0        0        0      157 2023-05-02 20:21:55.000000 seeq-spy-187.2/seeq/base/system.py
--rw-rw-rw-   0        0        0     4788 2023-05-02 20:21:55.000000 seeq-spy-187.2/seeq/base/util.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.041390 seeq-spy-187.2/seeq/scripts/
--rw-rw-rw-   0        0        0    12250 2023-05-02 20:21:55.000000 seeq-spy-187.2/seeq/scripts/create_monitoring_alerts.py
--rw-rw-rw-   0        0        0    49636 2023-05-02 20:21:55.000000 seeq-spy-187.2/seeq/scripts/create_monitoring_workbook.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.062388 seeq-spy-187.2/seeq/spy/
--rw-rw-rw-   0        0        0     1912 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/__init__.py
--rw-rw-rw-   0        0        0    30199 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_common.py
--rw-rw-rw-   0        0        0     4687 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_config.py
--rw-rw-rw-   0        0        0     4424 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_datalab.py
--rw-rw-rw-   0        0        0     9686 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_errors.py
--rw-rw-rw-   0        0        0    48955 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_login.py
--rw-rw-rw-   0        0        0    92210 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_metadata.py
--rw-rw-rw-   0        0        0     5822 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_metadata_push_results.py
--rw-rw-rw-   0        0        0     2954 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_plot.py
--rw-rw-rw-   0        0        0    55502 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_pull.py
--rw-rw-rw-   0        0        0    68554 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_push.py
--rw-rw-rw-   0        0        0     5155 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_redaction.py
--rw-rw-rw-   0        0        0    41144 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_search.py
--rw-rw-rw-   0        0        0    18978 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_session.py
--rw-rw-rw-   0        0        0    15704 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_status.py
--rw-rw-rw-   0        0        0     3471 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_upgrade.py
--rw-rw-rw-   0        0        0    10707 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/_url.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.066390 seeq-spy-187.2/seeq/spy/acl/
--rw-rw-rw-   0        0        0      104 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/acl/__init__.py
--rw-rw-rw-   0        0        0    12125 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/acl/_pull.py
--rw-rw-rw-   0        0        0    11313 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/acl/_push.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.074389 seeq-spy-187.2/seeq/spy/addons/
--rw-rw-rw-   0        0        0      188 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/addons/__init__.py
--rw-rw-rw-   0        0        0    26338 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/addons/_install.py
--rw-rw-rw-   0        0        0     2408 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/addons/_permissions.py
--rw-rw-rw-   0        0        0    12099 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/addons/_search.py
--rw-rw-rw-   0        0        0     5296 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/addons/_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.081390 seeq-spy-187.2/seeq/spy/assets/
--rw-rw-rw-   0        0        0      336 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_brochure.py
--rw-rw-rw-   0        0        0    12106 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_build.py
--rw-rw-rw-   0        0        0     3133 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_context.py
--rw-rw-rw-   0        0        0    48189 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_model.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.094389 seeq-spy-187.2/seeq/spy/assets/_trees/
--rw-rw-rw-   0        0        0       69 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/__init__.py
--rw-rw-rw-   0        0        0     1375 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_constants.py
--rw-rw-rw-   0        0        0     7302 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_csv.py
--rw-rw-rw-   0        0        0    22068 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_match.py
--rw-rw-rw-   0        0        0     2629 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_pandas.py
--rw-rw-rw-   0        0        0     6458 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_path.py
--rw-rw-rw-   0        0        0    23200 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_properties.py
--rw-rw-rw-   0        0        0    13341 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_pull.py
--rw-rw-rw-   0        0        0    58690 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_tree.py
--rw-rw-rw-   0        0        0     5885 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_utils.py
--rw-rw-rw-   0        0        0    25528 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/_trees/_validate.py
--rw-rw-rw-   0        0        0     2538 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/assets/brochure.html
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.098390 seeq-spy-187.2/seeq/spy/docs/
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.123391 seeq-spy-187.2/seeq/spy/docs/Documentation/
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.132390 seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/
--rw-rw-rw-   0        0        0    17105 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
--rw-rw-rw-   0        0        0    33412 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
--rw-rw-rw-   0        0        0    16369 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
--rw-rw-rw-   0        0        0     8406 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
--rw-rw-rw-   0        0        0    38705 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
--rw-rw-rw-   0        0        0      870 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
--rw-rw-rw-   0        0        0   184883 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
--rw-rw-rw-   0        0        0   222294 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
--rw-rw-rw-   0        0        0   228822 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
--rw-rw-rw-   0        0        0    24422 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.147390 seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/
--rw-rw-rw-   0        0        0   135771 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
--rw-rw-rw-   0        0        0   152116 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
--rw-rw-rw-   0        0        0   207271 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
--rw-rw-rw-   0        0        0      325 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/Readme.txt
--rw-rw-rw-   0        0        0   141516 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
--rw-rw-rw-   0        0        0   439966 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
--rw-rw-rw-   0        0        0   189377 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
--rw-rw-rw-   0        0        0    15176 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Command Reference.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.162392 seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/
--rw-rw-rw-   0        0        0    94677 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/Example Export.zip
--rw-rw-rw-   0        0        0   111771 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
--rw-rw-rw-   0        0        0   113084 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
--rw-rw-rw-   0        0        0  1083835 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
--rw-rw-rw-   0        0        0      429 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
--rw-rw-rw-   0        0        0   673871 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Tutorial.ipynb
--rw-rw-rw-   0        0        0    11411 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Version Considerations.ipynb
--rw-rw-rw-   0        0        0  1556967 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/Workbook Templates.ipynb
--rw-rw-rw-   0        0        0    53885 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/spy.acl.ipynb
--rw-rw-rw-   0        0        0    11009 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/spy.jobs.ipynb
--rw-rw-rw-   0        0        0    12828 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/spy.login.ipynb
--rw-rw-rw-   0        0        0   127929 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/spy.pull.ipynb
--rw-rw-rw-   0        0        0    99356 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/spy.push.ipynb
--rw-rw-rw-   0        0        0    54441 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/spy.search.ipynb
--rw-rw-rw-   0        0        0    10645 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/spy.widgets.ipynb
--rw-rw-rw-   0        0        0    69641 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/Documentation/spy.workbooks.ipynb
--rw-rw-rw-   0        0        0       60 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/docs/_copy.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.170390 seeq-spy-187.2/seeq/spy/jobs/
--rw-rw-rw-   0        0        0      491 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/jobs/__init__.py
--rw-rw-rw-   0        0        0     9869 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/jobs/_execute.py
--rw-rw-rw-   0        0        0     6111 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/jobs/_pull.py
--rw-rw-rw-   0        0        0     9362 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/jobs/_push.py
--rw-rw-rw-   0        0        0    25680 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/jobs/_schedule.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.174390 seeq-spy-187.2/seeq/spy/notifications/
--rw-rw-rw-   0        0        0      153 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/notifications/__init__.py
--rw-rw-rw-   0        0        0    11926 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/notifications/_emails.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.175389 seeq-spy-187.2/seeq/spy/utils/
--rw-rw-rw-   0        0        0     1569 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.178389 seeq-spy-187.2/seeq/spy/widgets/
--rw-rw-rw-   0        0        0      200 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/widgets/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/widgets/_ipy_utils.py
--rw-rw-rw-   0        0        0    30480 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/widgets/_widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.230391 seeq-spy-187.2/seeq/spy/workbooks/
--rw-rw-rw-   0        0        0     3012 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/__init__.py
--rw-rw-rw-   0        0        0    43676 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_annotation.py
--rw-rw-rw-   0        0        0    34087 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_content.py
--rw-rw-rw-   0        0        0    40535 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_data.py
--rw-rw-rw-   0        0        0     6677 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_folder.py
--rw-rw-rw-   0        0        0    14959 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_item.py
--rw-rw-rw-   0        0        0     5448 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_item_map.py
--rw-rw-rw-   0        0        0     3033 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_load.py
--rw-rw-rw-   0        0        0     3456 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_mustache.py
--rw-rw-rw-   0        0        0    14137 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_pull.py
--rw-rw-rw-   0        0        0    23050 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_push.py
--rw-rw-rw-   0        0        0     6316 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_render.py
--rw-rw-rw-   0        0        0    27127 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_report_content_utilities.py
--rw-rw-rw-   0        0        0     4729 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_save.py
--rw-rw-rw-   0        0        0    15507 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_search.py
--rw-rw-rw-   0        0        0    37445 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_template.py
--rw-rw-rw-   0        0        0    11995 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_user.py
--rw-rw-rw-   0        0        0    52393 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_workbook.py
--rw-rw-rw-   0        0        0    48744 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_worksheet.py
--rw-rw-rw-   0        0        0    50418 2023-05-02 20:21:57.000000 seeq-spy-187.2/seeq/spy/workbooks/_workstep.py
--rw-rw-rw-   0        0        0   427362 2023-05-02 20:21:56.000000 seeq-spy-187.2/seeq/spy/workbooks/app.css
-drwxrwxrwx   0        0        0        0 2023-05-02 20:22:00.245389 seeq-spy-187.2/seeq_spy.egg-info/
--rw-rw-rw-   0        0        0     4606 2023-05-02 20:21:59.000000 seeq-spy-187.2/seeq_spy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4660 2023-05-02 20:21:59.000000 seeq-spy-187.2/seeq_spy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 20:21:59.000000 seeq-spy-187.2/seeq_spy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-29 18:05:03.000000 seeq-spy-187.2/seeq_spy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      311 2023-05-02 20:21:59.000000 seeq-spy-187.2/seeq_spy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-02 20:21:59.000000 seeq-spy-187.2/seeq_spy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 20:22:00.247388 seeq-spy-187.2/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-05-02 20:19:46.000000 seeq-spy-187.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.442211 seeq-spy-187.5/
+-rw-rw-rw-   0        0        0    33551 2023-05-17 17:28:06.000000 seeq-spy-187.5/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-05-17 17:28:06.000000 seeq-spy-187.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4606 2023-05-17 17:45:36.441209 seeq-spy-187.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4091 2023-05-17 17:28:06.000000 seeq-spy-187.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.109225 seeq-spy-187.5/seeq/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.413213 seeq-spy-187.5/seeq/base/
+-rw-rw-rw-   0        0        0       36 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/proputil.py
+-rw-rw-rw-   0        0        0    32236 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/seeq_names.py
+-rw-rw-rw-   0        0        0      157 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/system.py
+-rw-rw-rw-   0        0        0     4788 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/base/util.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.414216 seeq-spy-187.5/seeq/scripts/
+-rw-rw-rw-   0        0        0    12250 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/scripts/create_monitoring_alerts.py
+-rw-rw-rw-   0        0        0    49636 2023-05-17 17:45:24.000000 seeq-spy-187.5/seeq/scripts/create_monitoring_workbook.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.426215 seeq-spy-187.5/seeq/spy/
+-rw-rw-rw-   0        0        0     1912 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/__init__.py
+-rw-rw-rw-   0        0        0    30851 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_common.py
+-rw-rw-rw-   0        0        0     4687 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_config.py
+-rw-rw-rw-   0        0        0     4424 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_datalab.py
+-rw-rw-rw-   0        0        0     9686 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_errors.py
+-rw-rw-rw-   0        0        0    48955 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_login.py
+-rw-rw-rw-   0        0        0    92210 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_metadata.py
+-rw-rw-rw-   0        0        0     5822 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_metadata_push_results.py
+-rw-rw-rw-   0        0        0     2954 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_plot.py
+-rw-rw-rw-   0        0        0    55502 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_pull.py
+-rw-rw-rw-   0        0        0    68554 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_push.py
+-rw-rw-rw-   0        0        0     5155 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_redaction.py
+-rw-rw-rw-   0        0        0    41144 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_search.py
+-rw-rw-rw-   0        0        0    18978 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_session.py
+-rw-rw-rw-   0        0        0    15704 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_status.py
+-rw-rw-rw-   0        0        0     3471 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_upgrade.py
+-rw-rw-rw-   0        0        0    10707 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/_url.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.427219 seeq-spy-187.5/seeq/spy/acl/
+-rw-rw-rw-   0        0        0      104 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/acl/__init__.py
+-rw-rw-rw-   0        0        0    12125 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/acl/_pull.py
+-rw-rw-rw-   0        0        0    11313 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/acl/_push.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.503212 seeq-spy-187.5/seeq/spy/addons/
+-rw-rw-rw-   0        0        0      188 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/__init__.py
+-rw-rw-rw-   0        0        0    26338 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/_install.py
+-rw-rw-rw-   0        0        0     2408 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/_permissions.py
+-rw-rw-rw-   0        0        0    12099 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/_search.py
+-rw-rw-rw-   0        0        0     5296 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/addons/_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.659217 seeq-spy-187.5/seeq/spy/assets/
+-rw-rw-rw-   0        0        0      336 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_brochure.py
+-rw-rw-rw-   0        0        0    12106 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_build.py
+-rw-rw-rw-   0        0        0     3133 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_context.py
+-rw-rw-rw-   0        0        0    48189 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_model.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.816216 seeq-spy-187.5/seeq/spy/assets/_trees/
+-rw-rw-rw-   0        0        0       69 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/__init__.py
+-rw-rw-rw-   0        0        0     1375 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_constants.py
+-rw-rw-rw-   0        0        0     7302 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_csv.py
+-rw-rw-rw-   0        0        0    22068 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_match.py
+-rw-rw-rw-   0        0        0     2629 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_pandas.py
+-rw-rw-rw-   0        0        0     6458 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_path.py
+-rw-rw-rw-   0        0        0    23200 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_properties.py
+-rw-rw-rw-   0        0        0    13341 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_pull.py
+-rw-rw-rw-   0        0        0    58690 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_tree.py
+-rw-rw-rw-   0        0        0     5885 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_utils.py
+-rw-rw-rw-   0        0        0    25528 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/_trees/_validate.py
+-rw-rw-rw-   0        0        0     2538 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/assets/brochure.html
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.817210 seeq-spy-187.5/seeq/spy/docs/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.917210 seeq-spy-187.5/seeq/spy/docs/Documentation/
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:35.919212 seeq-spy-187.5/seeq/spy/docs/Documentation/Administration/
+-rw-rw-rw-   0        0        0     6702 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.114216 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/
+-rw-rw-rw-   0        0        0    17428 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
+-rw-rw-rw-   0        0        0    33412 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
+-rw-rw-rw-   0        0        0    16700 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
+-rw-rw-rw-   0        0        0     8406 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
+-rw-rw-rw-   0        0        0    38705 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
+-rw-rw-rw-   0        0        0      870 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
+-rw-rw-rw-   0        0        0   184883 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
+-rw-rw-rw-   0        0        0   222294 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
+-rw-rw-rw-   0        0        0   228823 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
+-rw-rw-rw-   0        0        0    24442 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.182202 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/
+-rw-rw-rw-   0        0        0   135771 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
+-rw-rw-rw-   0        0        0   152116 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
+-rw-rw-rw-   0        0        0   207271 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
+-rw-rw-rw-   0        0        0      325 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/Readme.txt
+-rw-rw-rw-   0        0        0   141516 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
+-rw-rw-rw-   0        0        0   439966 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
+-rw-rw-rw-   0        0        0   189377 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
+-rw-rw-rw-   0        0        0    15176 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Command Reference.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.286207 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/
+-rw-rw-rw-   0        0        0    94677 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Example Export.zip
+-rw-rw-rw-   0        0        0   111771 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
+-rw-rw-rw-   0        0        0   113084 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
+-rw-rw-rw-   0        0        0  1083835 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
+-rw-rw-rw-   0        0        0      429 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
+-rw-rw-rw-   0        0        0   673873 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Tutorial.ipynb
+-rw-rw-rw-   0        0        0    11411 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Version Considerations.ipynb
+-rw-rw-rw-   0        0        0  1556967 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/Workbook Templates.ipynb
+-rw-rw-rw-   0        0        0    53885 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.acl.ipynb
+-rw-rw-rw-   0        0        0    11009 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.jobs.ipynb
+-rw-rw-rw-   0        0        0    12828 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.login.ipynb
+-rw-rw-rw-   0        0        0   127929 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.pull.ipynb
+-rw-rw-rw-   0        0        0    99356 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.push.ipynb
+-rw-rw-rw-   0        0        0    54441 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.search.ipynb
+-rw-rw-rw-   0        0        0    10645 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.widgets.ipynb
+-rw-rw-rw-   0        0        0    69641 2023-05-17 17:45:28.000000 seeq-spy-187.5/seeq/spy/docs/Documentation/spy.workbooks.ipynb
+-rw-rw-rw-   0        0        0       60 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/docs/_copy.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.292209 seeq-spy-187.5/seeq/spy/jobs/
+-rw-rw-rw-   0        0        0      491 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/_execute.py
+-rw-rw-rw-   0        0        0     6111 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/_pull.py
+-rw-rw-rw-   0        0        0     9362 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/_push.py
+-rw-rw-rw-   0        0        0    25680 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/jobs/_schedule.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.295206 seeq-spy-187.5/seeq/spy/notifications/
+-rw-rw-rw-   0        0        0      153 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/notifications/__init__.py
+-rw-rw-rw-   0        0        0    11926 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/notifications/_emails.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.297214 seeq-spy-187.5/seeq/spy/utils/
+-rw-rw-rw-   0        0        0     1569 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.300207 seeq-spy-187.5/seeq/spy/widgets/
+-rw-rw-rw-   0        0        0      200 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/widgets/_ipy_utils.py
+-rw-rw-rw-   0        0        0    30480 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/widgets/_widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.376205 seeq-spy-187.5/seeq/spy/workbooks/
+-rw-rw-rw-   0        0        0     3012 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/__init__.py
+-rw-rw-rw-   0        0        0    43676 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_annotation.py
+-rw-rw-rw-   0        0        0    34087 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_content.py
+-rw-rw-rw-   0        0        0    40535 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_data.py
+-rw-rw-rw-   0        0        0     6677 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_folder.py
+-rw-rw-rw-   0        0        0    14959 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_item.py
+-rw-rw-rw-   0        0        0     5448 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_item_map.py
+-rw-rw-rw-   0        0        0     3033 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_load.py
+-rw-rw-rw-   0        0        0     3456 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_mustache.py
+-rw-rw-rw-   0        0        0    14137 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_pull.py
+-rw-rw-rw-   0        0        0    23050 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_push.py
+-rw-rw-rw-   0        0        0     6316 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_render.py
+-rw-rw-rw-   0        0        0    27127 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_report_content_utilities.py
+-rw-rw-rw-   0        0        0     4729 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_save.py
+-rw-rw-rw-   0        0        0    15507 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_search.py
+-rw-rw-rw-   0        0        0    37445 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_template.py
+-rw-rw-rw-   0        0        0    11995 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_user.py
+-rw-rw-rw-   0        0        0    52393 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_workbook.py
+-rw-rw-rw-   0        0        0    48744 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_worksheet.py
+-rw-rw-rw-   0        0        0    51518 2023-05-17 17:45:33.000000 seeq-spy-187.5/seeq/spy/workbooks/_workstep.py
+-rw-rw-rw-   0        0        0   427362 2023-05-17 17:45:29.000000 seeq-spy-187.5/seeq/spy/workbooks/app.css
+drwxrwxrwx   0        0        0        0 2023-05-17 17:45:36.438218 seeq-spy-187.5/seeq_spy.egg-info/
+-rw-rw-rw-   0        0        0     4606 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4724 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      311 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-17 17:45:34.000000 seeq-spy-187.5/seeq_spy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 17:45:36.442211 seeq-spy-187.5/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-05-17 17:33:09.000000 seeq-spy-187.5/setup.py
```

### Comparing `seeq-spy-187.2/LICENSE` & `seeq-spy-187.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/PKG-INFO` & `seeq-spy-187.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 187.2
+Version: 187.5
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-187.2/README.md` & `seeq-spy-187.5/README.md`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/base/proputil.py` & `seeq-spy-187.5/seeq/base/proputil.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/base/seeq_names.py` & `seeq-spy-187.5/seeq/base/seeq_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,17 @@
         content = 'Content'
         report_templates = 'ReportTemplates'
         condition_monitors = 'ConditionMonitors'
         plugins = 'Plugins'
         displays = 'Displays'
         display_templates = 'DisplayTemplates'
         notification_configurations = 'NotificationConfigurations'
+        context = 'Context'
         table_definitions = 'TableDefinitions'
+        graph_q_l = 'GraphQL'
     
     class Channels:
         agents_status = 'agents-status'
         datasources_status = 'datasources-status'
         broadcast = 'broadcast'
         live_screenshot = 'live-screenshot'
         async_response = 'async-response'
@@ -305,15 +307,18 @@
         date_ranges = '/date-ranges'
         asset_selections = '/asset-selections'
         plugins = '/plugins'
         displays = '/displays'
         display_templates = '/display-templates'
         usage = '/usage'
         notification_configurations = '/notification-configurations'
+        labels = '/labels'
+        context = '/context'
         table_definitions = '/table-definitions'
+        graph_q_l = '/graphql'
         class ErrorMessages:
             attempted_to_set_scope_on_a_globally_scoped_item = 'Attempted to set scope on a globally scoped item'
         
         class AddOnToolLinkType:
             window = 'window'
             tab = 'tab'
             none = 'none'
@@ -456,14 +461,15 @@
         project_link = 'ProjectLink'
         add_on_tool = 'AddOnTool'
         base_annotation = 'BaseAnnotation'
         report = 'Report'
         report_template = 'ReportTemplate'
         journal = 'Journal'
         reply = 'Reply'
+        item_finder = 'ItemFinder'
         condition = 'Condition'
         condition_monitor = 'ConditionMonitor'
         capsule = 'Capsule'
         stored_condition = 'StoredCondition'
         calculated_condition = 'CalculatedCondition'
         scalar = 'ScalarItem'
         literal_scalar = 'LiteralScalar'
@@ -550,14 +556,15 @@
         archived_reason = 'Archived Reason'
         sync_token = 'Sync Token'
         number_format = 'Number Format'
         source_number_format = 'Source Number Format'
         string_format = 'String Format'
         source_string_format = 'Source String Format'
         storage_location = 'Storage Location'
+        executor_id = 'Executor ID'
         creator_id = 'Creator ID'
         creator_first_name = 'Creator First Name'
         creator_last_name = 'Creator Last Name'
         historical_data_version = 'Historical Data Version'
         manual_cdc = 'Manual CDC'
         scoped_to = 'Scoped To'
         asset = 'asset'
@@ -609,15 +616,15 @@
         previous_index_at = 'Previous Index At'
         sync_result = 'Sync Result'
         indexing_schedule_supported = 'Indexing Schedule Supported'
         asset_tree_search_index_needs_updating = 'Asset Tree Search Index Needs Updating'
         sync_mode = 'Sync Mode'
         items_archived_count = 'Items Archived Count'
         indexing_duration = 'Indexing Duration'
-        current_indexing_started_at = 'Current Indexing Started At'
+        indexing_progress_timestamp = 'Indexing Progress Timestamp'
         asset_progress = 'Asset Progress'
         asset_count = 'Asset Count'
         previous_asset_count = 'Previous Asset Count'
         signal_progress = 'Signal Progress'
         signal_count = 'Signal Count'
         previous_signal_count = 'Previous Signal Count'
         condition_progress = 'Condition Progress'
@@ -738,14 +745,16 @@
         summary_value = 'Summary Value'
         current_filename = 'Current Filename'
         last_result_hash = 'Last Result Hash'
         asset_path_depth = 'Asset Path Depth'
         last_run_at = 'Last Run At'
         last_run_state = 'Last Run State'
         query_range_look_ahead = 'Query Range Look Ahead'
+        finder_configurations = 'Finder Configurations'
+        last_run_warnings = 'Last Run Warnings'
         resource_size = 'Resource Size'
         project_type = 'Project Type'
         cron_schedule = 'Cron Schedule'
         background = 'Background'
         condition_formula_now = 'Condition Formula Now'
         notebook_path = 'Notebook Path'
         previous_run_time = 'Previous Run Time'
```

### Comparing `seeq-spy-187.2/seeq/base/util.py` & `seeq-spy-187.5/seeq/base/util.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/scripts/create_monitoring_alerts.py` & `seeq-spy-187.5/seeq/scripts/create_monitoring_alerts.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/scripts/create_monitoring_workbook.py` & `seeq-spy-187.5/seeq/scripts/create_monitoring_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/__init__.py` & `seeq-spy-187.5/seeq/spy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 """
 
 __all__ = ['acl', 'addons', 'assets', 'docs', 'workbooks', 'widgets', 'login', 'logout', 'plot', 'pull', 'push',
            'search', 'PATH_ROOT', 'DEFAULT_WORKBOOK_PATH', 'GLOBALS_ONLY', 'GLOBALS_AND_ALL_WORKBOOKS',
            'INHERIT_FROM_WORKBOOK', 'Session', 'Status', 'options', 'session', 'client', 'user', 'server_version',
            'jobs', 'notifications', 'upgrade', 'utils', 'errors']
 
-__version__ = '%d.%d' % (int('187'), int('2'))
+__version__ = '%d.%d' % (int('187'), int('5'))
```

### Comparing `seeq-spy-187.2/seeq/spy/_common.py` & `seeq-spy-187.5/seeq/spy/_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 import string
 import sys
 import traceback
 import types
 import uuid
 import warnings as pywarnings
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pytz
 from IPython.core.getipython import get_ipython
 from IPython.display import display, clear_output
 from deprecated import deprecated
@@ -382,23 +382,35 @@
     return datetime.datetime.now()
 
 
 def timer_elapsed(timer):
     return datetime.datetime.now() - timer
 
 
-def convert_to_timestamp(unix_timestamp_in_ns, tz):
-    return convert_timestamp_timezone(none_to_nan(pd.Timestamp(unix_timestamp_in_ns)), tz)
+def convert_to_timestamp(value: Union[int, str], tz: Optional[str]) -> pd.Timestamp:
+    """
+    :param value: A date/time in either nanoseconds from the Unix Epoch or as ISO-8601 string (with time zone).
+    :param tz: The time zone identifier to localize the value.
+    :return: The value as a localized pd.Timestamp. pd.NA and None values return as NA.
+    """
+    if pd.isna(value):
+        return pd.NA
+    elif isinstance(value, str):
+        value = pd.to_datetime(value)
+    elif not isinstance(value, (int, float)):
+        raise TypeError(f'Cannot convert {value} to timestamp. Expected either int or str.')
+    return convert_timestamp_timezone(none_to_nan(pd.Timestamp(value)), tz)
 
 
-def convert_timestamp_timezone(timestamp, tz):
+def convert_timestamp_timezone(timestamp: pd.Timestamp, tz: Optional[str]) -> pd.Timestamp:
     if pd.isna(timestamp):
         return timestamp
 
-    timestamp = timestamp.tz_localize('UTC')
+    if timestamp.tzinfo is None:
+        timestamp = timestamp.tz_localize('UTC')
     return timestamp.tz_convert(tz) if tz else timestamp
 
 
 def print_output(output: str):
     if is_rkernel():
         import rpy2.robjects as robjects
         rcode = f"cat('{output}')"
```

### Comparing `seeq-spy-187.2/seeq/spy/_config.py` & `seeq-spy-187.5/seeq/spy/_config.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_datalab.py` & `seeq-spy-187.5/seeq/spy/_datalab.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_errors.py` & `seeq-spy-187.5/seeq/spy/_errors.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_login.py` & `seeq-spy-187.5/seeq/spy/_login.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_metadata.py` & `seeq-spy-187.5/seeq/spy/_metadata.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_metadata_push_results.py` & `seeq-spy-187.5/seeq/spy/_metadata_push_results.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_plot.py` & `seeq-spy-187.5/seeq/spy/_plot.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_pull.py` & `seeq-spy-187.5/seeq/spy/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_push.py` & `seeq-spy-187.5/seeq/spy/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_redaction.py` & `seeq-spy-187.5/seeq/spy/_redaction.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_search.py` & `seeq-spy-187.5/seeq/spy/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_session.py` & `seeq-spy-187.5/seeq/spy/_session.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_status.py` & `seeq-spy-187.5/seeq/spy/_status.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_upgrade.py` & `seeq-spy-187.5/seeq/spy/_upgrade.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/_url.py` & `seeq-spy-187.5/seeq/spy/_url.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/acl/_pull.py` & `seeq-spy-187.5/seeq/spy/acl/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/acl/_push.py` & `seeq-spy-187.5/seeq/spy/acl/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/addons/_install.py` & `seeq-spy-187.5/seeq/spy/addons/_install.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/addons/_permissions.py` & `seeq-spy-187.5/seeq/spy/addons/_permissions.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/addons/_search.py` & `seeq-spy-187.5/seeq/spy/addons/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/addons/_uninstall.py` & `seeq-spy-187.5/seeq/spy/addons/_uninstall.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_brochure.py` & `seeq-spy-187.5/seeq/spy/assets/_brochure.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_build.py` & `seeq-spy-187.5/seeq/spy/assets/_build.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_context.py` & `seeq-spy-187.5/seeq/spy/assets/_context.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_model.py` & `seeq-spy-187.5/seeq/spy/assets/_model.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_constants.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_constants.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_csv.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_csv.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_match.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_match.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_pandas.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_pandas.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_path.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_path.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_properties.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_properties.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_pull.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_tree.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_tree.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_utils.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/_trees/_validate.py` & `seeq-spy-187.5/seeq/spy/assets/_trees/_validate.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/assets/brochure.html` & `seeq-spy-187.5/seeq/spy/assets/brochure.html`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999062860438293%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(0, \'# Email Notification Add-on Installer\\n\'), (3, "If '*

 * *            "you are using Seeq's SaaS product, instead of this Data Lab-based notification "*

 * *            'mechanism, it is recommended that you utilize the built in notification capabilities '*

 * *            'in Seeq R60+ as described in the following Seeq Knowledge Base article: '*

 * *            'https://support.seeq.com/space/KB/2594111502/Notifications+on+Conditions\\n"), (4, '*

 * *            "'\\n'), (5, 'This n […]*

```diff
@@ -1,18 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "5627e45a",
             "metadata": {},
             "source": [
-                "# Installer for Email Notification Scheduler\n",
+                "# Email Notification Add-on Installer\n",
                 "\u26a0\ufe0f Only Seeq Administrators can run this installer to completion, since only Administrators can install Add-ons.\n",
                 "\n",
-                "This notebook will walk you through the steps needed to install the Email Notification Scheduler as a Data Lab Tool in Workbench.  If you are fine with the defaults and have never installed the scheduler before, you should be able to leave everything as is, running all cells in order.   \n",
+                "If you are using Seeq's SaaS product, instead of this Data Lab-based notification mechanism, it is recommended that you utilize the built in notification capabilities in Seeq R60+ as described in the following Seeq Knowledge Base article: https://support.seeq.com/space/KB/2594111502/Notifications+on+Conditions\n",
+                "\n",
+                "This notebook will walk you through the steps needed to install the Email Notification Scheduler as a Data Lab Tool in Workbench. If you are fine with the defaults and have never installed the scheduler before, you should be able to leave everything as is, running all cells in order.\n",
                 "\n",
                 "At the end, if you have encountered no errors:\n",
                 "* in the folder you've specified using the `path_to_notifications_folder`, you should find all files listed as `source_files` below \n",
                 "* the Tools tab in Workbench should have a tool grouping named `Add-ons`\n",
                 "* there should be a tool named `Email Notification Scheduler` among the `Add-ons`.\n",
                 "\n",
                 "There is ONE MORE STEP that must be done to complete installation - after running all steps in this installer, one must complete the SMTP server and account configuration in `Email Notifier.ipynb` within the target folder (`Email Notifications` if `path_to_notifications_folder` is not changed below).  Please note that anyone that has access to this project will be able to see the account information provided there.  If using the gmail SMTP server, it is preferred to use an app password rather than the actual password for the account, and the port should be set to 587 to use STARTTLS.  You can find out more about gmail app passwords in the [Google Account Help](https://support.google.com/accounts/answer/185833?hl=en#zippy=%2Cwhy-you-may-need-an-app-password).\n",
@@ -128,15 +130,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2ee52e66",
             "metadata": {},
             "source": [
-                "# \u26a0\ufe0f Advanced Configuration and Automated Installation Beyond This Point\n",
+                "## \u26a0\ufe0f Advanced Configuration and Automated Installation Beyond This Point\n",
                 "If you are just running this notebook to install or update the Email Notifications Scheduler in a typical fashion, you can just run the remaining cells as is, checking the output of each to confirm the expected results.  Contact support if any problems are encountered."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fe06909b",
```

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999702380952381%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, "If you are using Seeq\'s SaaS product, instead of '*

 * *            'this Data Lab-based notification mechanism, it is recommended that you utilize the '*

 * *            'built in notification capabilities in Seeq R60+ as described in the following Seeq '*

 * *            'Knowledge Base article: '*

 * *            'https://support.seeq.com/space/KB/2594111502/Notifications+on+Conditions\\n"), (3, '*

 * *            "'\\n'), (4, 'This Notebook is intended to be scheduled from `Email No […]*

```diff
@@ -3,15 +3,17 @@
         {
             "cell_type": "markdown",
             "id": "af9e2356",
             "metadata": {},
             "source": [
                 "# Email Notifier\n",
                 "\n",
-                "This Notebook is intended to be scheduled from `Email Notification Scheduler.ipynb`.  Before using this Notifier, you will need to configure the connection to the email server.  Upon updating the following cell with appropriate credentials, uncomment the line\n",
+                "If you are using Seeq's SaaS product, instead of this Data Lab-based notification mechanism, it is recommended that you utilize the built in notification capabilities in Seeq R60+ as described in the following Seeq Knowledge Base article: https://support.seeq.com/space/KB/2594111502/Notifications+on+Conditions\n",
+                "\n",
+                "This Notebook is intended to be scheduled from `Email Notification Scheduler.ipynb`. Before using this Notifier, you will need to configure the connection to the email server. Upon updating the following cell with appropriate credentials, uncomment the line\n",
                 "\n",
                 "`# test_email()`\n",
                 "\n",
                 "so that it reads\n",
                 "\n",
                 "`test_email()`\n",
                 "\n",
```

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998647186147186%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'This tutorial leverages the capabilities of the "*

 * *            '**spy.assets** templates (as described in [Asset Trees 2 - '*

 * *            'Templates](Asset%20Trees%202%20-%20Templates.ipynb)) and **spy.workbooks** templates '*

 * *            '(as described in [Workbook Templates](Workbook%20Templates.ipynb)) to show you how to '*

 * *            'create Displays, Analysis Workbooks/Worksheets and Organizer Topics for your asset '*

 * *            "tree.\\n')], delete: [2]}}}"}*

```diff
@@ -47,15 +47,15 @@
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "# Asset Trees 3: Report and Dashboard Templates\n",
                 "\n",
-                "This tutorial leverages the capabilities of the **spy.assets** templates (as described in [Asset Trees 2 - Templates](Asset%20Trees%202%20-%20Templates.ipynb)) and **spy.workbooks** templates (as described in [Workbook Templates](Workbook%20Templates.ipynb)) to show you how to create Displays, Analysis Wrkbooks/Worksheets and Organizer Topics for your asset tree.\n",
+                "This tutorial leverages the capabilities of the **spy.assets** templates (as described in [Asset Trees 2 - Templates](Asset%20Trees%202%20-%20Templates.ipynb)) and **spy.workbooks** templates (as described in [Workbook Templates](Workbook%20Templates.ipynb)) to show you how to create Displays, Analysis Workbooks/Worksheets and Organizer Topics for your asset tree.\n",
                 "\n",
                 "First, some definitions:\n",
                 "\n",
                 "- **Display**: The definition of a visualization that can be rendered in Seeq Workbench. A Display can be a Trend, XY Plot, Treemap or Table. Technically speaking, a Display corresponds to what Seeq refers to internally as a **Workstep**.\n",
                 "- **Document**: In Seeq Organizer, each \"worksheet\" on the left-hand side of the display is called a Topic _Document_. Documents have rich text, images, and embedded content (called _Displays_ in this context) with associated Date Ranges and Asset Selections.\n",
                 "- **Asset**: An organizing unit / container that typically encapsulates Signals, Conditions, Scalars. They can also encapsulate the aforementioned Display and Document definitions.\n",
                 "\n",
```

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99817354826546%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, '# Asset Trees 4: Creating Accelerator Templates\\n')], "*

 * *            'delete: [0]}}, 3: {\'source\': {insert: [(0, \'## "Requirements"\\n\')], delete: '*

 * *            "[0]}}, 6: {'source': {insert: [(0, '## Analytics!\\n')], delete: [0]}}, 8: {'source': "*

 * *            "{insert: [(0, '## Input Tree\\n')], delete: [0]}}, 10: {'source': {insert: [(0, '## "*

 * *            "Build and Push\\n')], delete: [0]}}, 14: {'source': {insert: [(0, '## "*

 * *            "Brochures\\n')], d […]*

```diff
@@ -38,15 +38,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "coral-house",
             "metadata": {},
             "source": [
-                "# Creating Accelerator Templates\n",
+                "# Asset Trees 4: Creating Accelerator Templates\n",
                 "\n",
                 "The Seeq platform provides the basis for doing all sorts of analytics -- leveraging Seeq Workbench, Seeq Organizer, Seeq Data Lab -- with Seeq Cortex providing data connection and calculation capabilities.\n",
                 "\n",
                 "It can be useful for the Seeq community of partners and users to create _accelerators_ that deploy proven, standardized analytic approaches in rapid fashion using SPy's asset/workbook/topic templating capabilities in `spy.assets`. For example, an expert in monitoring and optimizing large-scale HVAC installations might develop an _Accelerator Template_ to deploy a set of useful calculations, visualizations and reports or dashboards that can handle variations in manufacturer, configuration etc and provide immediate value that can be expanded and built upon over time.\n",
                 "\n",
                 "This notebook illustrates how to use `spy.assets` infrastructure to create Accelerator Templates. If you haven't used it before, it is recommended that you first explore the following:\n",
                 "\n",
@@ -57,15 +57,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "little-humanitarian",
             "metadata": {},
             "source": [
-                "# \"Requirements\"\n",
+                "## \"Requirements\"\n",
                 "\n",
                 "The most important concept with Accelerator Templates is **Requirements**. A Requirement specifies an \"input\" to the template -- something that must be provided in order for the template to function. For example, if the template needs an ambient temperature signal in order to calculate an operational efficiency metric, that temperature signal is a Requirement. Furthermore, the operating limits may need to be provided, or perhaps the manufacturer/model of the equipment. These Requirements are the things that vary from installation to installation. The template can be written to adjust to these variations as long as it has the inputs it needs.\n",
                 "\n",
                 "Requirements are specified in a class like so:"
             ]
         },
         {
@@ -119,15 +119,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "stone-client",
             "metadata": {},
             "source": [
-                "# Analytics!\n",
+                "## Analytics!\n",
                 "\n",
                 "Now let's create a simple class that makes use of these two requirements. In this example, an `Inefficient Operation` condition is calculated by comparing `Compressor Power` and `Temperature` against hard-coded limits. (Such limits should likely be determined by manufacturer specifications or process control limits, but for now we'll keep it simple.)\n",
                 "\n",
                 "Note how this new `HVAC_Monitoring` class is derived from the `HVAC_Monitoring_Requirements`. This allows the `Inefficient Operation` calculation to refer to the members of the requirements class."
             ]
         },
         {
@@ -167,15 +167,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bridal-olive",
             "metadata": {},
             "source": [
-                "# Input Tree\n",
+                "## Input Tree\n",
                 "\n",
                 "The template is applied to an existing _input tree_. This tree must already be constructed, in whatever way makes sense for a particular use case. It may be different in each application of the template -- different hierarchy, different organization. The template will be applied to the tree as it is constructed, and any roll-ups will correspond to the particular hierarchy present in the input tree.\n",
                 "\n",
                 "In this example, we will use the **Example** asset tree that comes with Seeq. So we assemble a _metadata DataFrame_ by doing `spy.search(recursive=True)`."
             ]
         },
         {
@@ -337,15 +337,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ecological-parts",
             "metadata": {},
             "source": [
-                "# Build and Push\n",
+                "## Build and Push\n",
                 "\n",
                 "As with other uses of `spy.assets`, we must now build and then push the results."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
@@ -401,15 +401,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "satellite-gossip",
             "metadata": {},
             "source": [
-                "# Brochures\n",
+                "## Brochures\n",
                 "\n",
                 "Once you have an accelerator created, you can generate a _brochure_ that advertises the cool analytics that the accelerator provides.\n",
                 "\n",
                 "Execute the `spy.assets.brochure()` function like so:"
             ]
         },
         {
```

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Command Reference.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Command Reference.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/Example Export.zip` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Example Export.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Tutorial.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995659722222222%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '## Getting Started\\n')], delete: [0]}}, 17: {'source': "*

 * *            '{insert: [(0, "## Using Seeq\'s Calculation Engine\\n")], delete: [0]}}}'}*

```diff
@@ -12,15 +12,15 @@
                 "This tutorial walks you through the basics of searching for data, getting it into a DataFrame and then writing it back to a Seeq Workbench workbook."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Getting Started\n",
+                "## Getting Started\n",
                 "This section will walk you through searching for signals in Seeq and pulling data.\n",
                 "\n",
                 "## Importing the SPy Module\n",
                 "The **SPy** module (short for Seeq PYthon) is what you'll use to interact with Seeq Server and access data. Start by importing it."
             ]
         },
         {
@@ -553,15 +553,15 @@
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Using Seeq's Calculation Engine\n",
+                "## Using Seeq's Calculation Engine\n",
                 "\n",
                 "What if we want to use Seeq's calculation engine to reduce the noise in the **Temperature** and **Relative Humidity** signals?\n",
                 "\n",
                 "We can apply a calculation by specifying a formula as the `calculation` argument."
             ]
         },
         {
```

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Version Considerations.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Version Considerations.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/Workbook Templates.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/Workbook Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/spy.acl.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.acl.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/spy.jobs.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/spy.login.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.login.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/spy.pull.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.pull.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/spy.push.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.push.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/spy.search.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.search.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/spy.widgets.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.widgets.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/Documentation/spy.workbooks.ipynb` & `seeq-spy-187.5/seeq/spy/docs/Documentation/spy.workbooks.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/docs/_copy.py` & `seeq-spy-187.5/seeq/spy/docs/_copy.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/jobs/_execute.py` & `seeq-spy-187.5/seeq/spy/jobs/_execute.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/jobs/_pull.py` & `seeq-spy-187.5/seeq/spy/jobs/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/jobs/_push.py` & `seeq-spy-187.5/seeq/spy/jobs/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/jobs/_schedule.py` & `seeq-spy-187.5/seeq/spy/jobs/_schedule.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/notifications/_emails.py` & `seeq-spy-187.5/seeq/spy/notifications/_emails.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/utils/__init__.py` & `seeq-spy-187.5/seeq/spy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/widgets/_ipy_utils.py` & `seeq-spy-187.5/seeq/spy/widgets/_ipy_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/widgets/_widgets.py` & `seeq-spy-187.5/seeq/spy/widgets/_widgets.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/__init__.py` & `seeq-spy-187.5/seeq/spy/workbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_annotation.py` & `seeq-spy-187.5/seeq/spy/workbooks/_annotation.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_content.py` & `seeq-spy-187.5/seeq/spy/workbooks/_content.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_data.py` & `seeq-spy-187.5/seeq/spy/workbooks/_data.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_folder.py` & `seeq-spy-187.5/seeq/spy/workbooks/_folder.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_item.py` & `seeq-spy-187.5/seeq/spy/workbooks/_item.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_item_map.py` & `seeq-spy-187.5/seeq/spy/workbooks/_item_map.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_load.py` & `seeq-spy-187.5/seeq/spy/workbooks/_load.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_mustache.py` & `seeq-spy-187.5/seeq/spy/workbooks/_mustache.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_pull.py` & `seeq-spy-187.5/seeq/spy/workbooks/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_push.py` & `seeq-spy-187.5/seeq/spy/workbooks/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_render.py` & `seeq-spy-187.5/seeq/spy/workbooks/_render.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_report_content_utilities.py` & `seeq-spy-187.5/seeq/spy/workbooks/_report_content_utilities.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_save.py` & `seeq-spy-187.5/seeq/spy/workbooks/_save.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_search.py` & `seeq-spy-187.5/seeq/spy/workbooks/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_template.py` & `seeq-spy-187.5/seeq/spy/workbooks/_template.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_user.py` & `seeq-spy-187.5/seeq/spy/workbooks/_user.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_workbook.py` & `seeq-spy-187.5/seeq/spy/workbooks/_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_worksheet.py` & `seeq-spy-187.5/seeq/spy/workbooks/_worksheet.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/_workstep.py` & `seeq-spy-187.5/seeq/spy/workbooks/_workstep.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,16 +351,25 @@
         See worksheet properties "display_range" for docs
         :return:
         """
         duration_store = self._get_store('sqDurationStore')
         display_range = _common.get(duration_store, 'displayRange', default=dict())
         if not display_range:
             return None
-        start = _common.convert_to_timestamp(display_range['start'] * 1000000, 'UTC')
-        end = _common.convert_to_timestamp(display_range['end'] * 1000000, 'UTC')
+        try:
+            # Note: If the frontend stores the values as numeric, it's Epoch seconds rather than ns.
+            start_raw = display_range['start']
+            start_val = start_raw * 1_000_000 if not isinstance(start_raw, str) else start_raw
+            start = _common.convert_to_timestamp(start_val, 'UTC')
+            end_raw = display_range['end']
+            end_val = end_raw * 1_000_000 if not isinstance(end_raw, str) else end_raw
+            end = _common.convert_to_timestamp(end_val, 'UTC')
+        except BaseException as e:
+            raise SPyValueError(f'Error parsing Display Range. '
+                                f'Times must be numeric or valid ISO8601 strings.') from e
         return {'Start': start, 'End': end}
 
     def set_display_range(self, display_start_end, check_investigate=True, session: Optional[Session] = None):
         """
         Set the display range
 
         See worksheet properties "display_range" for docs
@@ -418,16 +427,25 @@
         See worksheet property "investigate_range" for docs
         :return:
         """
         duration_store = self._get_store('sqDurationStore')
         investigate_range = _common.get(duration_store, 'investigateRange', default=None)
         if investigate_range is None:
             return None
-        start = _common.convert_to_timestamp(investigate_range['start'] * 1000000, 'UTC')
-        end = _common.convert_to_timestamp(investigate_range['end'] * 1000000, 'UTC')
+        try:
+            # Note: If the frontend stores the values as numeric, it's Epoch seconds rather than ns.
+            start_raw = investigate_range['start']
+            start_val = start_raw * 1_000_000 if not isinstance(start_raw, str) else start_raw
+            start = _common.convert_to_timestamp(start_val, 'UTC')
+            end_raw = investigate_range['end']
+            end_val = end_raw * 1_000_000 if not isinstance(end_raw, str) else end_raw
+            end = _common.convert_to_timestamp(end_val, 'UTC')
+        except BaseException as e:
+            raise SPyValueError(f'Error parsing Investigate Range. '
+                                f'Times must be numeric or valid ISO8601 strings.') from e
         return {'Start': start, 'End': end}
 
     def set_investigate_range(self, investigate_start_end, check_display=True, session: Optional[Session] = None):
         """
         Set the investigate range
 
         See worksheet property "investigate_range" for docs
```

### Comparing `seeq-spy-187.2/seeq/spy/workbooks/app.css` & `seeq-spy-187.5/seeq/spy/workbooks/app.css`

 * *Files identical despite different names*

### Comparing `seeq-spy-187.2/seeq_spy.egg-info/PKG-INFO` & `seeq-spy-187.5/seeq_spy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 187.2
+Version: 187.5
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-187.2/seeq_spy.egg-info/SOURCES.txt` & `seeq-spy-187.5/seeq_spy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 seeq/spy/docs/Documentation/spy.jobs.ipynb
 seeq/spy/docs/Documentation/spy.login.ipynb
 seeq/spy/docs/Documentation/spy.pull.ipynb
 seeq/spy/docs/Documentation/spy.push.ipynb
 seeq/spy/docs/Documentation/spy.search.ipynb
 seeq/spy/docs/Documentation/spy.widgets.ipynb
 seeq/spy/docs/Documentation/spy.workbooks.ipynb
+seeq/spy/docs/Documentation/Administration/User Migration.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
 seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
 seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
```

### Comparing `seeq-spy-187.2/setup.py` & `seeq-spy-187.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq-spy",
-    version="187.2",
+    version="187.5",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="Easy-to-use Python interface for Seeq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```


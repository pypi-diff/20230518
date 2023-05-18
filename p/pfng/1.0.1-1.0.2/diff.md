# Comparing `tmp/pfng-1.0.1.tar.gz` & `tmp/pfng-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfng-1.0.1.tar", last modified: Sat May  6 14:42:23 2023, max compression
+gzip compressed data, was "pfng-1.0.2.tar", last modified: Thu May 18 20:07:36 2023, max compression
```

## Comparing `pfng-1.0.1.tar` & `pfng-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 14:42:23.374567 pfng-1.0.1/
--rw-rw-rw-   0        0        0     1093 2023-05-02 20:33:55.000000 pfng-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       25 2023-05-06 14:03:46.000000 pfng-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2546 2023-05-06 14:42:23.374567 pfng-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1915 2023-05-06 14:40:53.000000 pfng-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 14:42:23.368115 pfng-1.0.1/pfng/
--rw-rw-rw-   0        0        0       69 2023-05-04 19:19:10.000000 pfng-1.0.1/pfng/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:42:23.373568 pfng-1.0.1/pfng/data/
--rw-rw-rw-   0        0        0     1535 2023-04-30 19:51:52.000000 pfng-1.0.1/pfng/data/female_names.csv
--rw-rw-rw-   0        0        0   131363 2023-05-01 13:40:19.000000 pfng-1.0.1/pfng/data/female_surnames.csv
--rw-rw-rw-   0        0        0     1270 2023-04-30 19:49:43.000000 pfng-1.0.1/pfng/data/male_names.csv
--rw-rw-rw-   0        0        0   134570 2023-05-01 13:40:26.000000 pfng-1.0.1/pfng/data/male_surnames.csv
--rw-rw-rw-   0        0        0      853 2023-05-06 14:20:41.000000 pfng-1.0.1/pfng/data_reader.py
--rw-rw-rw-   0        0        0     1058 2023-05-06 14:20:53.000000 pfng-1.0.1/pfng/generator.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:42:23.370565 pfng-1.0.1/pfng.egg-info/
--rw-rw-rw-   0        0        0     2546 2023-05-06 14:42:23.000000 pfng-1.0.1/pfng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-06 14:42:23.000000 pfng-1.0.1/pfng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 14:42:23.000000 pfng-1.0.1/pfng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-06 14:42:23.000000 pfng-1.0.1/pfng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 14:42:23.374567 pfng-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-05-06 14:41:31.000000 pfng-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:07:36.679382 pfng-1.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-05-02 20:33:55.000000 pfng-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       52 2023-05-18 19:43:25.000000 pfng-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3366 2023-05-18 20:07:36.679382 pfng-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2720 2023-05-18 19:50:30.000000 pfng-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 20:07:36.669384 pfng-1.0.2/pfng/
+-rw-rw-rw-   0        0        0       26 2023-05-18 18:26:51.000000 pfng-1.0.2/pfng/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-18 18:25:48.000000 pfng-1.0.2/pfng/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:07:36.678398 pfng-1.0.2/pfng/data/
+-rw-rw-rw-   0        0        0     1520 2023-05-18 19:05:04.000000 pfng-1.0.2/pfng/data/female_names.csv
+-rw-rw-rw-   0        0        0   131345 2023-05-18 19:05:11.000000 pfng-1.0.2/pfng/data/female_surnames.csv
+-rw-rw-rw-   0        0        0     1251 2023-05-18 19:05:16.000000 pfng-1.0.2/pfng/data/male_names.csv
+-rw-rw-rw-   0        0        0   134548 2023-05-18 19:05:22.000000 pfng-1.0.2/pfng/data/male_surnames.csv
+-rw-rw-rw-   0        0        0      796 2023-05-18 19:05:39.000000 pfng-1.0.2/pfng/data_reader.py
+-rw-rw-rw-   0        0        0     1197 2023-05-18 19:33:15.000000 pfng-1.0.2/pfng/generator.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:07:36.672382 pfng-1.0.2/pfng.egg-info/
+-rw-rw-rw-   0        0        0     3366 2023-05-18 20:07:36.000000 pfng-1.0.2/pfng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-18 20:07:36.000000 pfng-1.0.2/pfng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 20:07:36.000000 pfng-1.0.2/pfng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-18 20:07:36.000000 pfng-1.0.2/pfng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 20:07:36.679382 pfng-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3189 2023-05-18 20:06:05.000000 pfng-1.0.2/setup.py
```

### Comparing `pfng-1.0.1/LICENSE` & `pfng-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pfng-1.0.1/PKG-INFO` & `pfng-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,89 @@
 Metadata-Version: 2.1
 Name: pfng
-Version: 1.0.1
-Summary: Polish full names generator
-Home-page: https://github.com/JakubPrz/Polish-Full-Names-Generator
+Version: 1.0.2
+Summary: Full name generator powered by thousands of Polish names and surnames. Both male and female full names can be generated.
+Home-page: https://github.com/JakubPrz/Polish-Full-Name-Generator
 Author: Jakub Przepiórka
 Author-email: jakub.przepiorka.contact.me@gmail.com
 License: MIT
 Platform: Windows
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
-Classifier: Natural Language :: English
 Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Polish Full Names Generator
-**Author:** Jakub Przepiórka \
-**Version:** 1.0.1
+# Polish Full Name Generator
+Author: Jakub Przepiórka 
+Version: 1.0.2
+
 
 ## About
-The generator is powered by thousands of Polish names and surnames, which allows you to create many thousands of combinations of unique full names.
+The pfng is powered by thousands of Polish names and surnames, which allows you to generate thousands combinations of unique full names.
+You can choose whether you want to generate male or female full names or mix of them.
+
+Why it is useful tool?
+- Forget about inventing or manually typing names and surnames. This polish full name generator can generate you quickly thousands of full names.
+- It can be useful when generating fake data or testing some applications.
 
-You can choose whether you want to generate male or female full names or both of them.
+No dependencies 
+This package does not depend on other modules or packages that are not already included in standard Python distributions.
 
-This generator can help quickly insert thousands of users to database, rather than having to manually enter names for each person. It can also be useful when testing booking systems or other applications.
+Operating system 
+This package is written to work on Windows. There is no guarantee that it will work on other operating systems.
 
-Programming language: Python
 
 ## Installation
-~~Install it using pip:~~ \
-~~> `pip3 install ...`~~
+The preferred channel is [PyPI](https://pypi.org/project/pfng/):
+```
+pip install pfng
+```
+
+Alternatively, you can clone GitHub [repository](https://github.com/JakubPrz/Polish-Full-Name-Generator):
+```
+git clone git@github.com:JakubPrz/Polish-Full-Name-Generator.git
+```
 
-Or clone this repository:
-> `git clone git@github.com:JakubPrz/Polish-Full-Names-Generator.git`
 
 ## Usage
 ```python
-from pfng.generator import generate_full_names
+from pfng import generate_full_names
+
 
 people = generate_full_names(number=20, gender='M&F')
 
-# ex1: you can print them
+# Example 1: you can print them
 for p in people:
     print(p)
 
-# ex2: or save them to file
-with open("generated_full_names.txt", mode="w", encoding="utf-8") as file:
+# Example 2: save them to file for later use
+with open("full_names.txt", mode="w", encoding="utf-8") as file:
     for f in people:
-        file.write(f + "\n")
+        file.write(f + "n")
 ```
 
-## Generated people sample
-*['Waldemar Jastrząb', 'Marek Suliński', 'Nela Orawiec', 'Dagmara Czeczko', 'Aneta Makaruk', 'Laura Krężel', 'Janusz Gumułka', 'Iza Łuka', 'Ala Orzeł', 'Roksana Pilichowska', 'Nela Berus', 'Lila Gabryel', 'Mateusz Czopor', 'Alfred Dorsz', 'Anna Kanabus', 'Jerzy Bojek', 'Szymon Prędki', 'Adam Pondel', 'Julian Wichary', 'Sylwester Ogrodowczyk', 'Kajetan Parka', 'Witold Purtak', 'Urszula Opałka', 'Kazimiera Zawół', 'Ola Kuskowska', 'Szczepan Tokaj', 'Edward Pasierbek', 'Tymon Pielach', 'Maurycy Block', 'Remigiusz Wasiela']*
+The ```gender``` parameter options:
+
+| Option | Meaning                           |
+|--------|-----------------------------------|
+| M      | Only male full names              |
+| F      | Only female full names            |
+| M&F    | Mix of male and female full names |
+
+
+## Generated full names sample
+['Waldemar Jastrząb', 'Marek Suliński', 'Nela Orawiec', 'Dagmara Czeczko', 'Aneta Makaruk', 'Laura Krężel', 'Janusz Gumułka', 'Iza Łuka', 'Ala Orzeł', 'Roksana Pilichowska', 'Nela Berus', 'Lila Gabryel', 'Mateusz Czopor', 'Alfred Dorsz', 'Anna Kanabus', 'Jerzy Bojek', 'Szymon Prędki', 'Adam Pondel', 'Julian Wichary', 'Sylwester Ogrodowczyk', 'Kajetan Parka', 'Witold Purtak', 'Urszula Opałka', 'Kazimiera Zawół', 'Ola Kuskowska', 'Szczepan Tokaj', 'Edward Pasierbek', 'Tymon Pielach', 'Maurycy Block', 'Remigiusz Wasiela']
+
+Note: There are only Polish full names because it's Polish Full Name Generator.
+
 
 ## Contributing
-Contributions are welcome! \
+Contributions are welcome! 
 If you would like to make any improvements to this generator, feel free to submit a pull request.
 
+
 ## License
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License - see the LICENSE.md file for details.
```

### Comparing `pfng-1.0.1/README.md` & `pfng-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,71 @@
-# Polish Full Names Generator
+# Polish Full Name Generator
 **Author:** Jakub Przepiórka \
-**Version:** 1.0.1
+**Version:** 1.0.2
+
 
 ## About
-The generator is powered by thousands of Polish names and surnames, which allows you to create many thousands of combinations of unique full names.
+The pfng is powered by thousands of Polish names and surnames, which allows you to generate thousands combinations of unique full names.
+You can choose whether you want to generate male or female full names or mix of them.
+
+**Why it is useful tool?**
+- Forget about inventing or manually typing names and surnames. This polish full name generator can generate you quickly thousands of full names.
+- It can be useful when generating fake data or testing some applications.
 
-You can choose whether you want to generate male or female full names or both of them.
+**No dependencies** \
+This package does not depend on other modules or packages that are not already included in standard Python distributions.
 
-This generator can help quickly insert thousands of users to database, rather than having to manually enter names for each person. It can also be useful when testing booking systems or other applications.
+**Operating system** \
+This package is written to work on Windows. There is no guarantee that it will work on other operating systems.
 
-Programming language: Python
 
 ## Installation
-~~Install it using pip:~~ \
-~~> `pip3 install ...`~~
+The preferred channel is [PyPI](https://pypi.org/project/pfng/):
+```
+pip install pfng
+```
+
+Alternatively, you can clone GitHub [repository](https://github.com/JakubPrz/Polish-Full-Name-Generator):
+```
+git clone git@github.com:JakubPrz/Polish-Full-Name-Generator.git
+```
 
-Or clone this repository:
-> `git clone git@github.com:JakubPrz/Polish-Full-Names-Generator.git`
 
 ## Usage
 ```python
-from pfng.generator import generate_full_names
+from pfng import generate_full_names
+
 
 people = generate_full_names(number=20, gender='M&F')
 
-# ex1: you can print them
+# Example 1: you can print them
 for p in people:
     print(p)
 
-# ex2: or save them to file
-with open("generated_full_names.txt", mode="w", encoding="utf-8") as file:
+# Example 2: save them to file for later use
+with open("full_names.txt", mode="w", encoding="utf-8") as file:
     for f in people:
         file.write(f + "\n")
 ```
 
-## Generated people sample
+The ```gender``` parameter options:
+
+| Option | Meaning                           |
+|--------|-----------------------------------|
+| M      | Only male full names              |
+| F      | Only female full names            |
+| M&F    | Mix of male and female full names |
+
+
+## Generated full names sample
 *['Waldemar Jastrząb', 'Marek Suliński', 'Nela Orawiec', 'Dagmara Czeczko', 'Aneta Makaruk', 'Laura Krężel', 'Janusz Gumułka', 'Iza Łuka', 'Ala Orzeł', 'Roksana Pilichowska', 'Nela Berus', 'Lila Gabryel', 'Mateusz Czopor', 'Alfred Dorsz', 'Anna Kanabus', 'Jerzy Bojek', 'Szymon Prędki', 'Adam Pondel', 'Julian Wichary', 'Sylwester Ogrodowczyk', 'Kajetan Parka', 'Witold Purtak', 'Urszula Opałka', 'Kazimiera Zawół', 'Ola Kuskowska', 'Szczepan Tokaj', 'Edward Pasierbek', 'Tymon Pielach', 'Maurycy Block', 'Remigiusz Wasiela']*
 
+**Note:** There are only **Polish** full names because it's Polish Full Name Generator.
+
+
 ## Contributing
 Contributions are welcome! \
 If you would like to make any improvements to this generator, feel free to submit a pull request.
 
+
 ## License
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License - see the LICENSE.md file for details.
```

### Comparing `pfng-1.0.1/pfng/data/female_names.csv` & `pfng-1.0.2/pfng/data/female_names.csv`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-IMIĘ_KOBIETA
 Ada
 Adrianna
 Agata
 Agnieszka
 Ala
 Aldona
 Aleksandra
```

### Comparing `pfng-1.0.1/pfng/data/female_surnames.csv` & `pfng-1.0.2/pfng/data/female_surnames.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-NAZWISKO_KOBIETA
 Abram
 Abramczuk
 Abramczyk
 Abramek
 Abramowicz
 Abramowska
 Abramska
```

### Comparing `pfng-1.0.1/pfng/data/male_names.csv` & `pfng-1.0.2/pfng/data/male_names.csv`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-IMIĘ_MĘŻCZYZNA
 Adam
 Adolf
 Adrian
 Alan
 Aleks
 Aleksander
 Alfred
```

### Comparing `pfng-1.0.1/pfng/data/male_surnames.csv` & `pfng-1.0.2/pfng/data/male_surnames.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-NAZWISKO_MĘŻCZYZNA
 Abram
 Abramczuk
 Abramczyk
 Abramek
 Abramowicz
 Abramowski
 Abramski
```

### Comparing `pfng-1.0.1/pfng/data_reader.py` & `pfng-1.0.2/pfng/data_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-from typing import List
 from pathlib import Path
+from typing import List
 from csv import reader
 
 
-def _read_from_csv(csv_path: str) -> List[str]:
+def _read_csv(csv_path: str) -> List[str]:
     """
-    Reads the data from a CSV file.
+    Reads data from a CSV file.
 
     Args:
         csv_path: The path of the CSV file.
 
     Returns:
-        A list of rows from the CSV file.
+        A list containing rows from the CSV file.
     """
     with open(csv_path, encoding="utf-8") as file:
         csv_reader = reader(file)
-        next(csv_reader)  # skip header
         rows = [r[0] for r in csv_reader]
     return rows
 
 
-data_dir = Path(__file__).parent / 'data'
+_data_dir = Path(__file__).parent / 'data'
 
-MALE_NAMES = _read_from_csv(Path(data_dir, 'male_names.csv').as_posix())
-FEMALE_NAMES = _read_from_csv(Path(data_dir, 'female_names.csv').as_posix())
-MALE_SURNAMES = _read_from_csv(Path(data_dir, 'male_surnames.csv').as_posix())
-FEMALE_SURNAMES = _read_from_csv(Path(data_dir, 'female_surnames.csv').as_posix())
+MALE_NAMES = _read_csv(Path(_data_dir, 'male_names.csv').as_posix())
+FEMALE_NAMES = _read_csv(Path(_data_dir, 'female_names.csv').as_posix())
+MALE_SURNAMES = _read_csv(Path(_data_dir, 'male_surnames.csv').as_posix())
+FEMALE_SURNAMES = _read_csv(Path(_data_dir, 'female_surnames.csv').as_posix())
```

### Comparing `pfng-1.0.1/pfng/generator.py` & `pfng-1.0.2/pfng/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,28 +8,32 @@
     Generates full names.
 
     Args:
         number: The number of full names to generate.
         gender (optional): The gender of full names (M, F, M&F)
 
     Raises:
+        ValueError: If number of full names is < 1
         TypeError: If invalid gender was given.
 
     Returns:
         full_names: A list of generated full names.
     """
 
     gender_map = {
         'M': (MALE_NAMES, MALE_SURNAMES),
         'F': (FEMALE_NAMES, FEMALE_SURNAMES),
         'M&F': None
     }
 
+    if number < 1:
+        raise ValueError('Number of full names must be > 0 !')
+
     if gender not in gender_map.keys():
-        raise TypeError("Provide valid gender type!")
+        raise TypeError('Provide valid gender type !')
 
     full_names = []
     for i in range(number):
         if gender == 'M&F':
             name_list, surname_list = gender_map[choice(['M', 'F'])]
         else:
             name_list, surname_list = gender_map[gender]
```

### Comparing `pfng-1.0.1/pfng.egg-info/PKG-INFO` & `pfng-1.0.2/pfng.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,89 @@
 Metadata-Version: 2.1
 Name: pfng
-Version: 1.0.1
-Summary: Polish full names generator
-Home-page: https://github.com/JakubPrz/Polish-Full-Names-Generator
+Version: 1.0.2
+Summary: Full name generator powered by thousands of Polish names and surnames. Both male and female full names can be generated.
+Home-page: https://github.com/JakubPrz/Polish-Full-Name-Generator
 Author: Jakub Przepiórka
 Author-email: jakub.przepiorka.contact.me@gmail.com
 License: MIT
 Platform: Windows
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
-Classifier: Natural Language :: English
 Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Polish Full Names Generator
-**Author:** Jakub Przepiórka \
-**Version:** 1.0.1
+# Polish Full Name Generator
+Author: Jakub Przepiórka 
+Version: 1.0.2
+
 
 ## About
-The generator is powered by thousands of Polish names and surnames, which allows you to create many thousands of combinations of unique full names.
+The pfng is powered by thousands of Polish names and surnames, which allows you to generate thousands combinations of unique full names.
+You can choose whether you want to generate male or female full names or mix of them.
+
+Why it is useful tool?
+- Forget about inventing or manually typing names and surnames. This polish full name generator can generate you quickly thousands of full names.
+- It can be useful when generating fake data or testing some applications.
 
-You can choose whether you want to generate male or female full names or both of them.
+No dependencies 
+This package does not depend on other modules or packages that are not already included in standard Python distributions.
 
-This generator can help quickly insert thousands of users to database, rather than having to manually enter names for each person. It can also be useful when testing booking systems or other applications.
+Operating system 
+This package is written to work on Windows. There is no guarantee that it will work on other operating systems.
 
-Programming language: Python
 
 ## Installation
-~~Install it using pip:~~ \
-~~> `pip3 install ...`~~
+The preferred channel is [PyPI](https://pypi.org/project/pfng/):
+```
+pip install pfng
+```
+
+Alternatively, you can clone GitHub [repository](https://github.com/JakubPrz/Polish-Full-Name-Generator):
+```
+git clone git@github.com:JakubPrz/Polish-Full-Name-Generator.git
+```
 
-Or clone this repository:
-> `git clone git@github.com:JakubPrz/Polish-Full-Names-Generator.git`
 
 ## Usage
 ```python
-from pfng.generator import generate_full_names
+from pfng import generate_full_names
+
 
 people = generate_full_names(number=20, gender='M&F')
 
-# ex1: you can print them
+# Example 1: you can print them
 for p in people:
     print(p)
 
-# ex2: or save them to file
-with open("generated_full_names.txt", mode="w", encoding="utf-8") as file:
+# Example 2: save them to file for later use
+with open("full_names.txt", mode="w", encoding="utf-8") as file:
     for f in people:
-        file.write(f + "\n")
+        file.write(f + "n")
 ```
 
-## Generated people sample
-*['Waldemar Jastrząb', 'Marek Suliński', 'Nela Orawiec', 'Dagmara Czeczko', 'Aneta Makaruk', 'Laura Krężel', 'Janusz Gumułka', 'Iza Łuka', 'Ala Orzeł', 'Roksana Pilichowska', 'Nela Berus', 'Lila Gabryel', 'Mateusz Czopor', 'Alfred Dorsz', 'Anna Kanabus', 'Jerzy Bojek', 'Szymon Prędki', 'Adam Pondel', 'Julian Wichary', 'Sylwester Ogrodowczyk', 'Kajetan Parka', 'Witold Purtak', 'Urszula Opałka', 'Kazimiera Zawół', 'Ola Kuskowska', 'Szczepan Tokaj', 'Edward Pasierbek', 'Tymon Pielach', 'Maurycy Block', 'Remigiusz Wasiela']*
+The ```gender``` parameter options:
+
+| Option | Meaning                           |
+|--------|-----------------------------------|
+| M      | Only male full names              |
+| F      | Only female full names            |
+| M&F    | Mix of male and female full names |
+
+
+## Generated full names sample
+['Waldemar Jastrząb', 'Marek Suliński', 'Nela Orawiec', 'Dagmara Czeczko', 'Aneta Makaruk', 'Laura Krężel', 'Janusz Gumułka', 'Iza Łuka', 'Ala Orzeł', 'Roksana Pilichowska', 'Nela Berus', 'Lila Gabryel', 'Mateusz Czopor', 'Alfred Dorsz', 'Anna Kanabus', 'Jerzy Bojek', 'Szymon Prędki', 'Adam Pondel', 'Julian Wichary', 'Sylwester Ogrodowczyk', 'Kajetan Parka', 'Witold Purtak', 'Urszula Opałka', 'Kazimiera Zawół', 'Ola Kuskowska', 'Szczepan Tokaj', 'Edward Pasierbek', 'Tymon Pielach', 'Maurycy Block', 'Remigiusz Wasiela']
+
+Note: There are only Polish full names because it's Polish Full Name Generator.
+
 
 ## Contributing
-Contributions are welcome! \
+Contributions are welcome! 
 If you would like to make any improvements to this generator, feel free to submit a pull request.
 
+
 ## License
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License - see the LICENSE.md file for details.
```


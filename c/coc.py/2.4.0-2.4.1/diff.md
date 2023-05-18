# Comparing `tmp/coc.py-2.4.0.tar.gz` & `tmp/coc.py-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coc.py-2.4.0.tar", last modified: Sun May 14 19:12:13 2023, max compression
+gzip compressed data, was "coc.py-2.4.1.tar", last modified: Thu May 18 19:36:05 2023, max compression
```

## Comparing `coc.py-2.4.0.tar` & `coc.py-2.4.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.286276 coc.py-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-14 19:11:58.000000 coc.py-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 19:11:58.000000 coc.py-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-14 19:12:13.286276 coc.py-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-14 19:11:58.000000 coc.py-2.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc/
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/clans.py
--rw-r--r--   0 runner    (1001) docker     (123)    80631 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/entry_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    39759 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/events.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.278276 coc.py-2.4.0/coc/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc/ext/discordlinks/
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/discordlinks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc/ext/fullwarapi/
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/fullwarapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc/ext/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/triggers/cron.py
--rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/ext/triggers/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/hero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22005 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/login.py
--rw-r--r--   0 runner    (1001) docker     (123)    21796 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/player_clan.py
--rw-r--r--   0 runner    (1001) docker     (123)    26903 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/players.py
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/raid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/spell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.286276 coc.py-2.4.0/coc/static/
--rw-r--r--   0 runner    (1001) docker     (123)   135500 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/buildings.json
--rw-r--r--   0 runner    (1001) docker     (123)   271286 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   130902 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/heroes.json
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/object_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    43766 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/pets.json
--rw-r--r--   0 runner    (1001) docker     (123)    53705 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/spells.json
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/supers.json
--rw-r--r--   0 runner    (1001) docker     (123)   575079 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/texts_EN.json
--rw-r--r--   0 runner    (1001) docker     (123)    41725 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/townhall_levels.json
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/static/update_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/troop.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/war_attack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/war_clans.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/war_members.py
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-05-14 19:11:58.000000 coc.py-2.4.0/coc/wars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:13.282276 coc.py-2.4.0/coc.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-14 19:12:13.000000 coc.py-2.4.0/coc.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-14 19:11:58.000000 coc.py-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 19:11:58.000000 coc.py-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 19:12:13.286276 coc.py-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 19:11:58.000000 coc.py-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.229443 coc.py-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-18 19:35:54.000000 coc.py-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 19:35:54.000000 coc.py-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-18 19:36:05.229443 coc.py-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-18 19:35:54.000000 coc.py-2.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/clans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80631 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/entry_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39786 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/events.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.221443 coc.py-2.4.1/coc/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc/ext/discordlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/discordlinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc/ext/fullwarapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/fullwarapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc/ext/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/triggers/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/ext/triggers/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/hero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22136 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21796 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/player_clan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26903 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/players.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/raid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/spell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.229443 coc.py-2.4.1/coc/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   135500 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/buildings.json
+-rw-r--r--   0 runner    (1001) docker     (123)   271286 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130902 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/heroes.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/object_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43766 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/pets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53705 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/spells.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/supers.json
+-rw-r--r--   0 runner    (1001) docker     (123)   575079 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/texts_EN.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41725 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/townhall_levels.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/static/update_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/troop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/war_attack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/war_clans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/war_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-05-18 19:35:54.000000 coc.py-2.4.1/coc/wars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:36:05.225443 coc.py-2.4.1/coc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-18 19:36:05.000000 coc.py-2.4.1/coc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 19:35:54.000000 coc.py-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 19:35:54.000000 coc.py-2.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:36:05.229443 coc.py-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 19:35:54.000000 coc.py-2.4.1/setup.py
```

### Comparing `coc.py-2.4.0/LICENSE` & `coc.py-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/PKG-INFO` & `coc.py-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 2.4.0
+Version: 2.4.1
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc.py-2.4.0/README.rst` & `coc.py-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/__init__.py` & `coc.py-2.4.1/coc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 from .abc import BasePlayer, BaseClan
 from .clans import RankedClan, Clan
 from .client import Client
 from .events import PlayerEvents, ClanEvents, WarEvents, EventsClient, ClientEvents
 from .enums import (
     PlayerHouseElementType,
```

### Comparing `coc.py-2.4.0/coc/abc.py` & `coc.py-2.4.1/coc/abc.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/clans.py` & `coc.py-2.4.1/coc/clans.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/client.py` & `coc.py-2.4.1/coc/client.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/entry_logs.py` & `coc.py-2.4.1/coc/entry_logs.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/enums.py` & `coc.py-2.4.1/coc/enums.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/errors.py` & `coc.py-2.4.1/coc/errors.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/events.py` & `coc.py-2.4.1/coc/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         except AttributeError:
             pass
 
         if self.cls.event_type == "client":
             return self.cls.__getattr__(self.cls, item)
 
         # handle member_x events:
-        if "member_" in item:
+        if "member_" in item and item != "member_count":
             item = item.replace("member_", "")
             nested = True
         else:
             nested = False
 
         return self._create_event(item.replace("_change", ""), nested)
```

### Comparing `coc.py-2.4.0/coc/events.pyi` & `coc.py-2.4.1/coc/events.pyi`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/ext/discordlinks/__init__.py` & `coc.py-2.4.1/coc/ext/discordlinks/__init__.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/ext/fullwarapi/__init__.py` & `coc.py-2.4.1/coc/ext/fullwarapi/__init__.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/ext/triggers/cron.py` & `coc.py-2.4.1/coc/ext/triggers/cron.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/ext/triggers/triggers.py` & `coc.py-2.4.1/coc/ext/triggers/triggers.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/hero.py` & `coc.py-2.4.1/coc/hero.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/http.py` & `coc.py-2.4.1/coc/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,16 +479,21 @@
             resp_payload = await resp.json()
             ip = json_loads(base64_b64decode(resp_payload["temporaryAPIToken"].split(".")[1] + "====").decode("utf-8"))["limits"][1]["cidrs"][0].split("/")[0]
 
             LOG.info("Found IP address to be %s", ip)
 
             resp = await session.post("https://developer.clashofclans.com/api/apikey/list")
             keys = (await resp.json())["keys"]
-            self._keys.extend(key["key"] for c, key in enumerate(keys) if key["name"] == self.key_names and ip in key[
-                "cidrRanges"] and c <= self.key_count)
+            for key in keys:
+                LOG.debug(f"Key {key}")
+                if key["name"] != self.key_names or ip not in key["cidrRanges"]:
+                    continue
+                self._keys.append(key["key"])
+                if len(self._keys) == self.key_count:
+                    break
 
             LOG.info("Retrieved %s valid keys from the developer site.", len(self._keys))
 
             if len(self._keys) < self.key_count:
                 for key in keys[:]:
                     if key["name"] != self.key_names or ip in key["cidrRanges"]:
                         continue
```

### Comparing `coc.py-2.4.0/coc/iterators.py` & `coc.py-2.4.1/coc/iterators.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/login.py` & `coc.py-2.4.1/coc/login.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/miscmodels.py` & `coc.py-2.4.1/coc/miscmodels.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/player_clan.py` & `coc.py-2.4.1/coc/player_clan.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/players.py` & `coc.py-2.4.1/coc/players.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/raid.py` & `coc.py-2.4.1/coc/raid.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/spell.py` & `coc.py-2.4.1/coc/spell.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/buildings.json` & `coc.py-2.4.1/coc/static/buildings.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/characters.json` & `coc.py-2.4.1/coc/static/characters.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/heroes.json` & `coc.py-2.4.1/coc/static/heroes.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/object_ids.json` & `coc.py-2.4.1/coc/static/object_ids.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/pets.json` & `coc.py-2.4.1/coc/static/pets.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/spells.json` & `coc.py-2.4.1/coc/static/spells.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/supers.json` & `coc.py-2.4.1/coc/static/supers.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/texts_EN.json` & `coc.py-2.4.1/coc/static/texts_EN.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/townhall_levels.json` & `coc.py-2.4.1/coc/static/townhall_levels.json`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/static/update_static.py` & `coc.py-2.4.1/coc/static/update_static.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/troop.py` & `coc.py-2.4.1/coc/troop.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/utils.py` & `coc.py-2.4.1/coc/utils.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/war_attack.py` & `coc.py-2.4.1/coc/war_attack.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/war_clans.py` & `coc.py-2.4.1/coc/war_clans.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/war_members.py` & `coc.py-2.4.1/coc/war_members.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc/wars.py` & `coc.py-2.4.1/coc/wars.py`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/coc.py.egg-info/PKG-INFO` & `coc.py-2.4.1/coc.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 2.4.0
+Version: 2.4.1
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc.py-2.4.0/coc.py.egg-info/SOURCES.txt` & `coc.py-2.4.1/coc.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coc.py-2.4.0/pyproject.toml` & `coc.py-2.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coc.py"
 authors = [{ name = "mathsman5133" }]
 maintainers = [{ name = "majordoobie" }, { name = "MagicTheDev" }, { name = "Kuchenmampfer" }, { name = "lukasthaler" }, { name = "doluk" }]
-version = "2.4.0"
+version = "2.4.1"
 description = "A python wrapper for the Clash of Clans API"
 requires-python = ">=3.7.3"
 readme = "README.rst"
 license = { text = "MIT" }
 keywords = ["coc", "clash of clans", "coc.py", "clash api"]
 classifiers = ["Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```


# Comparing `tmp/tidbcloudy-1.1.0a1.tar.gz` & `tmp/tidbcloudy-1.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidbcloudy-1.1.0a1.tar", max compression
+gzip compressed data, was "tidbcloudy-1.1.0a2.tar", max compression
```

## Comparing `tidbcloudy-1.1.0a1.tar` & `tidbcloudy-1.1.0a2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11342 2022-11-19 13:10:25.391866 tidbcloudy-1.1.0a1/LICENSE
--rw-r--r--   0        0        0    13758 2022-11-28 15:53:00.864074 tidbcloudy-1.1.0a1/README.md
--rw-r--r--   0        0        0      477 2022-12-04 15:05:53.764155 tidbcloudy-1.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      657 2022-11-28 16:09:33.896616 tidbcloudy-1.1.0a1/tidbcloudy/__init__.py
--rw-r--r--   0        0        0    11823 2022-12-04 14:56:00.597779 tidbcloudy-1.1.0a1/tidbcloudy/__main__.py
--rw-r--r--   0        0        0     4507 2022-11-28 14:52:17.384459 tidbcloudy-1.1.0a1/tidbcloudy/api/_base.py
--rw-r--r--   0        0        0     1579 2022-11-28 14:52:17.406505 tidbcloudy-1.1.0a1/tidbcloudy/api/backup.py
--rw-r--r--   0        0        0     8818 2022-12-04 14:34:01.121146 tidbcloudy-1.1.0a1/tidbcloudy/api/cluster.py
--rw-r--r--   0        0        0     2025 2022-12-04 09:11:45.879552 tidbcloudy-1.1.0a1/tidbcloudy/api/context.py
--rw-r--r--   0        0        0     9283 2022-11-28 14:52:17.400887 tidbcloudy-1.1.0a1/tidbcloudy/api/project.py
--rw-r--r--   0        0        0     1296 2022-11-28 14:52:17.397009 tidbcloudy-1.1.0a1/tidbcloudy/api/restore.py
--rw-r--r--   0        0        0    14584 2022-11-28 14:52:17.390718 tidbcloudy-1.1.0a1/tidbcloudy/api/specification.py
--rw-r--r--   0        0        0     4266 2022-12-04 09:38:18.381179 tidbcloudy-1.1.0a1/tidbcloudy/api/tidbcloud.py
--rw-r--r--   0        0        0      656 2022-11-28 16:09:33.893996 tidbcloudy-1.1.0a1/tidbcloudy/exception/__init__.py
--rw-r--r--   0        0        0      434 2022-08-14 14:52:41.153619 tidbcloudy-1.1.0a1/tidbcloudy/util/ip.py
--rw-r--r--   0        0        0      192 2022-08-14 14:52:41.153780 tidbcloudy-1.1.0a1/tidbcloudy/util/log.py
--rw-r--r--   0        0        0      541 2022-08-14 14:52:41.153967 tidbcloudy-1.1.0a1/tidbcloudy/util/page.py
--rw-r--r--   0        0        0      278 2022-08-14 14:52:41.154164 tidbcloudy-1.1.0a1/tidbcloudy/util/timestamp.py
--rw-r--r--   0        0        0    15041 1970-01-01 00:00:00.000000 tidbcloudy-1.1.0a1/setup.py
--rw-r--r--   0        0        0    14515 1970-01-01 00:00:00.000000 tidbcloudy-1.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2022-09-21 10:14:42.906372 tidbcloudy-1.1.0a2/LICENSE
+-rw-r--r--   0        0        0    13758 2022-11-29 09:15:58.046775 tidbcloudy-1.1.0a2/README.md
+-rw-r--r--   0        0        0      477 2022-12-05 02:55:56.284178 tidbcloudy-1.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0      657 2022-11-29 09:15:58.050176 tidbcloudy-1.1.0a2/tidbcloudy/__init__.py
+-rw-r--r--   0        0        0    11832 2022-12-05 02:43:55.174423 tidbcloudy-1.1.0a2/tidbcloudy/__main__.py
+-rw-r--r--   0        0        0     4507 2022-11-29 09:15:58.050641 tidbcloudy-1.1.0a2/tidbcloudy/api/_base.py
+-rw-r--r--   0        0        0     1579 2022-11-29 09:15:58.050802 tidbcloudy-1.1.0a2/tidbcloudy/api/backup.py
+-rw-r--r--   0        0        0     8818 2022-12-05 02:38:55.586286 tidbcloudy-1.1.0a2/tidbcloudy/api/cluster.py
+-rw-r--r--   0        0        0     2025 2022-12-05 02:38:55.586459 tidbcloudy-1.1.0a2/tidbcloudy/api/context.py
+-rw-r--r--   0        0        0     9283 2022-11-29 09:15:58.051664 tidbcloudy-1.1.0a2/tidbcloudy/api/project.py
+-rw-r--r--   0        0        0     1296 2022-11-29 09:15:58.051867 tidbcloudy-1.1.0a2/tidbcloudy/api/restore.py
+-rw-r--r--   0        0        0    14584 2022-11-29 09:15:58.052104 tidbcloudy-1.1.0a2/tidbcloudy/api/specification.py
+-rw-r--r--   0        0        0     4266 2022-12-05 02:38:55.586614 tidbcloudy-1.1.0a2/tidbcloudy/api/tidbcloud.py
+-rw-r--r--   0        0        0      656 2022-11-29 09:15:58.052597 tidbcloudy-1.1.0a2/tidbcloudy/exception/__init__.py
+-rw-r--r--   0        0        0      434 2022-08-15 03:21:27.398042 tidbcloudy-1.1.0a2/tidbcloudy/util/ip.py
+-rw-r--r--   0        0        0      192 2022-08-15 03:21:27.398228 tidbcloudy-1.1.0a2/tidbcloudy/util/log.py
+-rw-r--r--   0        0        0      541 2022-08-15 03:21:27.398341 tidbcloudy-1.1.0a2/tidbcloudy/util/page.py
+-rw-r--r--   0        0        0      278 2022-08-15 03:21:27.398535 tidbcloudy-1.1.0a2/tidbcloudy/util/timestamp.py
+-rw-r--r--   0        0        0    15035 2022-12-05 02:56:52.039022 tidbcloudy-1.1.0a2/setup.py
+-rw-r--r--   0        0        0    14464 2022-12-05 02:56:52.039509 tidbcloudy-1.1.0a2/PKG-INFO
```

### Comparing `tidbcloudy-1.1.0a1/LICENSE` & `tidbcloudy-1.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/README.md` & `tidbcloudy-1.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/__init__.py` & `tidbcloudy-1.1.0a2/tidbcloudy/__init__.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/__main__.py` & `tidbcloudy-1.1.0a2/tidbcloudy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,20 +40,20 @@
 def cli_cluster():
     pass
 
 
 @cli_cluster.command("create")
 @click.option("-f", "--file", help="The json configuration file")
 @click.pass_obj
-def cli_cluster_create(obj, f):
+def cli_cluster_create(obj, file):
     cluster_config = CreateClusterConfig()
     api = obj["api"]  # type: TiDBCloud
     project = obj["project"]  # type: Project
-    if f is not None:
-        cluster_config = json.load(f)
+    if file is not None:
+        cluster_config = json.load(file)
         new_cluster = project.create_cluster(cluster_config)
         click.echo(f"Creating the cluster...")
         new_cluster.wait_for_available()
         return
     cluster_type = click.prompt("Select cluster type",
                                 type=click.Choice([str(item.value) for item in ClusterType], case_sensitive=False))
     cluster_config.set_cluster_type(cluster_type)
```

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/api/_base.py` & `tidbcloudy-1.1.0a2/tidbcloudy/api/_base.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/api/backup.py` & `tidbcloudy-1.1.0a2/tidbcloudy/api/backup.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/api/cluster.py` & `tidbcloudy-1.1.0a2/tidbcloudy/api/cluster.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/api/context.py` & `tidbcloudy-1.1.0a2/tidbcloudy/api/context.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/api/project.py` & `tidbcloudy-1.1.0a2/tidbcloudy/api/project.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/api/restore.py` & `tidbcloudy-1.1.0a2/tidbcloudy/api/restore.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/api/specification.py` & `tidbcloudy-1.1.0a2/tidbcloudy/api/specification.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/api/tidbcloud.py` & `tidbcloudy-1.1.0a2/tidbcloudy/api/tidbcloud.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/exception/__init__.py` & `tidbcloudy-1.1.0a2/tidbcloudy/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/tidbcloudy/util/page.py` & `tidbcloudy-1.1.0a2/tidbcloudy/util/page.py`

 * *Files identical despite different names*

### Comparing `tidbcloudy-1.1.0a1/setup.py` & `tidbcloudy-1.1.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,22 +16,22 @@
  'toml>=0.10.2,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['tidbcloudy = tidbcloudy.__main__:cli']}
 
 setup_kwargs = {
     'name': 'tidbcloudy',
-    'version': '1.1.0a1',
+    'version': '1.1.0a2',
     'description': 'Python SDK for TiDB Cloud',
     'long_description': '# Python SDK for TiDB Cloud\n\n`tidbcloudy` is an unofficial Python SDK for [TiDB Cloud](https://tidbcloud.com).\n\n## Introduction\n\nFor more information about TiDB Cloud API, see [TiDB Cloud API Documentation](https://docs.pingcap.com/tidbcloud/api/v1beta).\n\n> TiDB Cloud is a fully-managed Database-as-a-Service (DBaaS) that brings everything great about TiDB to your cloud.\n\nIf you do not have a TiDB Cloud account yet, you can sign up [here](https://tidbcloud.com). For more details about TiDB Cloud, refer to [TiDB Cloud Documentation](https://docs.pingcap.com/tidbcloud/).\n\nYou can use this SDK to access [TiDB Cloud](https://tidbcloud.com) and manage your projects, clusters, backups and restores:\n\n- manage your TiDB Cloud **projects** (only _list_ is supported now)\n- list all available cloud providers (AWS and GCP), regions and specifications before creating or modifying a cluster\n- manage your Serverless Tier or Dedicated Tier **clusters** (_create_, _modify_, _pause_, _resume_, _get_, _list_, _delete_)\n- manage your **backups** of a cluster (_create_, _get_, _list_, _delete_)\n- manage your **restores** of a project (_create_, _get_, _list_)\n\n### Compatibility with TiDB Cloud API\n\n`tidbcloudy` is compatible with [TiDB Cloud API](https://docs.pingcap.com/tidbcloud/api/v1beta). The following table lists the supported API versions:\n\n| tidbcloudy                                                         | TiDB Cloud API                                                                                          |\n|--------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|\n| [1.0.1](https://github.com/Oreoxmt/tidbcloudy/releases/tag/v1.0.1) | v1beta [Release 20220906](https://docs.pingcap.com/tidbcloud/api/v1beta#section/API-Changelog/20220906), [Release 20220920](https://docs.pingcap.com/tidbcloud/api/v1beta#section/API-Changelog/20220920), [Release 20221028](https://docs.pingcap.com/tidbcloud/api/v1beta#section/API-Changelog/20221028)|\n| [1.0.0](https://github.com/Oreoxmt/tidbcloudy/releases/tag/v1.0.0) | v1beta [Release 20220823](https://docs.pingcap.com/tidbcloud/api/v1beta#section/API-Changelog/20220823) |\n| [0.2.1](https://github.com/Oreoxmt/tidbcloudy/releases/tag/v0.2.1) | v1beta [Release 20220809](https://docs.pingcap.com/tidbcloud/api/v1beta#section/API-Changelog/20220809) |                                                                          |\n\n### Enhancements comparing to original [TiDB Cloud API](https://docs.pingcap.com/tidbcloud/api/v1beta)\n\n- **Iterate over** resources instead of manual pagination\n- **Connect to a TiDB cluster** using the [MySQL client](https://github.com/PyMySQL/mysqlclient)\n- **Get** a Project using a Project **ID**\n- Configure your cluster with **method chaining**\n- Add your **current IP address automatically**\n- **Wait for the cluster to be ready** when creating/modifying a cluster\n- **Case-insensitive** when setting cluster type, cloud provider, and component name\n\n## Installation\n\n```bash\npip3 install tidbcloudy\n```\n\n⚠️ Make sure that you have installed **mysql client** in your environment. For more information, see [PyMySQL/mysqlclient](https://github.com/PyMySQL/mysqlclient#install).\n\n## Usage\n\n### Prerequisites\n\n- Create a TiDB Cloud account.\n- Create a TiDB Cloud API key. To manage your API keys, see [TiDB Cloud API Documentation](https://docs.pingcap.com/tidbcloud/api/v1beta#section/Authentication/API-Key-Management).\n- Install the latest version of `tidbcloudy`.\n\nTo get full code examples, see the [`examples`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples) folder.\n\n> Note:\n>\n> It is recommended to set environment variables for your API public and private key. For example, in bash, you can:\n>\n> ```bash\n> export PUBLIC_KEY=your_api_public_key\n> export PRIVATE_KEY=your_api_private_key\n> ```\n\n### List all resources in your organization\n\nTo get the full code example of listing all projects, clusters, backup tasks, and restore tasks in your organization, see [`0_list_resources.py`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples/0_list_resources.py).\n\n```python\nimport os\n\nimport tidbcloudy\nfrom tidbcloudy.api.specification import ClusterType\n\npublic_key = os.environ.get("PUBLIC_KEY")\nprivate_key = os.environ.get("PRIVATE_KEY")\n\napi = tidbcloudy.TiDBCloud(public_key=public_key, private_key=private_key)\n\nfor project in api.iter_projects():\n    print(project)\n    for cluster in project.iter_clusters():\n        print(cluster)\n        if cluster.cluster_type == ClusterType.DEDICATED:\n            for backup in cluster.iter_backups():\n                print(backup)\n    for restore in project.iter_restores():\n        print(restore)\n```\n\n### Create a cluster\n\nBefore creating a cluster, you should list all available provider regions and cluster configuration specifications. For more details, run the [`1_list_provider_regions.py`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples/1_list_provider_regions.py).\n\n```python\nimport os\n\nimport tidbcloudy\n\npublic_key = os.environ.get("PUBLIC_KEY")\nprivate_key = os.environ.get("PRIVATE_KEY")\n\napi = tidbcloudy.TiDBCloud(public_key=public_key, private_key=private_key)\n\nfor spec in api.list_provider_regions():\n    print(f"- type: {spec.cluster_type.value}")\n    print(f"  provider: {spec.cloud_provider.value}")\n    print(f"  region: {spec.region}")\n    print(f"  components:")\n    for tidb in spec.tidb:\n        print(f"  - tidb: {tidb.node_size}; "\n              f"min={tidb.node_quantity_range.min} step={tidb.node_quantity_range.step}")\n    for tikv in spec.tikv:\n        print(f"  - tikv: {tikv.node_size}; "\n              f"min={tikv.node_quantity_range.min} "\n              f"step={tikv.node_quantity_range.step}; "\n              f"{tikv.storage_size_gib_range.min}..{tikv.storage_size_gib_range.max} GiB")\n    for tiflash in spec.tiflash:\n        print(\n            f"  - tiflash: {tiflash.node_size}; "\n            f"min={tiflash.node_quantity_range.min} step={tiflash.node_quantity_range.step}; "\n            f"{tiflash.storage_size_gib_range.min}..{tiflash.storage_size_gib_range.max} GiB")\n```\n\n> Note:\n>\n> Creating a cluster might cost money. For more details, see [TiDB Cloud pricing details](https://www.pingcap.com/tidb-cloud-pricing-details/).\n\nTo create a Serverless Tier cluster, run the [`2_1_create_serverless_cluster.py`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples/2_1_create_serverless_cluster.py).\n\nTo create a Dedicated Tier cluster, run the [`2_2_create_dedicated_cluster.py`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples/2_2_create_dedicated_cluster.py).\n\nThe following takes creating a Serverless Tier cluster as an example:\n\n```python\nimport os\nimport tidbcloudy\nfrom tidbcloudy.api.specification import CreateClusterConfig\n\npublic_key = os.environ.get("PUBLIC_KEY")\nprivate_key = os.environ.get("PRIVATE_KEY")\ndebug_mode = os.environ.get("TIDBCLOUDY_LOG")\nproject_id = "1234567890123456789"\n\napi = tidbcloudy.TiDBCloud(public_key=public_key, private_key=private_key)\nproject = api.get_project(project_id, update_from_server=True)\n\nconfig = CreateClusterConfig()\nconfig \\\n    .set_name("serverless-0") \\\n    .set_cluster_type("DEVELOPER") \\\n    .set_cloud_provider("AWS") \\\n    .set_region("us-west-2") \\\n    .set_root_password("your_root_password") \\\n    .add_ip_access(cidr="0.0.0.0/0") \\\n    .add_current_ip_access()\ncluster = project.create_cluster(config)\nprint(cluster)\n\ncluster.wait_for_ready()\n```\n\n### Connect to TiDB\n\nTo connect to your TiDB cluster, run the [`3_connect_mysql.py`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples/3_connect_mysql.py).\n\n```python\nimport os\n\nimport tidbcloudy\nfrom tidbcloudy.api.specification import ClusterStatus\n\npublic_key = os.environ.get("PUBLIC_KEY")\nprivate_key = os.environ.get("PRIVATE_KEY")\nproject_id = "1234567890123456789"\ncluster_id = "1234567890123456789"\n\nprint("Connecting to TiDB Cloud...")\napi = tidbcloudy.TiDBCloud(public_key=public_key, private_key=private_key)\nproject = api.get_project(project_id, update_from_server=True)\ncluster = project.get_cluster(cluster_id)\nprint(cluster)\n\nif cluster.status.cluster_status == ClusterStatus.AVAILABLE:\n    connection_strings = cluster.status.connection_strings\n    connection = cluster.connect(type="standard", database="test", password="your_root_password")\n    print(connection)\n    with connection:\n        with connection.cursor() as cursor:\n            cursor.execute("SELECT DATABASE();")\n            m = cursor.fetchone()\n            print(m[0])\n```\n\n### Modify a cluster\n\n> Note:\n>\n> Modify a cluster might cost money. For more details, see [TiDB Cloud pricing details](https://www.pingcap.com/tidb-cloud-pricing-details/).\n\nTo modify a cluster, run the [`4_scale_a_cluster.py`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples/4_scale_a_cluster.py).\n\n```python\nimport os\n\nimport tidbcloudy\nfrom tidbcloudy.api.specification import UpdateClusterConfig\n\npublic_key = os.environ.get("PUBLIC_KEY")\nprivate_key = os.environ.get("PRIVATE_KEY")\nproject_id = "1234567890123456789"\ncluster_id = "1234567890123456789"\n\napi = tidbcloudy.TiDBCloud(public_key=public_key, private_key=private_key)\nproject = api.get_project(project_id, update_from_server=True)\ncluster = project.get_cluster(cluster_id)\n\nprint("The original config is: {}".format(cluster.config.components.to_object()))\n\nnew_config = UpdateClusterConfig()\nnew_config.update_component("tiflash", node_quantity=1, node_size="8C64G", storage_size_gib=500)\ncluster.update(new_config)\ncluster.wait_for_ready()\n\nprint("The new config is: {}".format(cluster.config.components.to_object()))\n```\n\n### Backup and restore\n\n> Note:\n>\n> Backup or restore a cluster might cost money. For more details, see [TiDB Cloud pricing details](https://www.pingcap.com/tidb-cloud-pricing-details/).\n\nTo create a backup and restore, run the [`5_backup_restore.py`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples/5_backup_restore.py)\n\n```python\nimport os\n\nimport tidbcloudy\nfrom tidbcloudy.api.specification import CreateClusterConfig\n\npublic_key = os.environ.get("PUBLIC_KEY")\nprivate_key = os.environ.get("PRIVATE_KEY")\nproject_id = "1234567890123456789"\ncluster_id = "1234567890123456789"\nbackup_id = "1234567"\n\napi = tidbcloudy.TiDBCloud(public_key=public_key, private_key=private_key)\nproject = api.get_project(project_id, update_from_server=True)\ncluster = project.get_cluster(cluster_id)\nprint("Create a manual backup task")\nbackup = cluster.create_backup(name="backup-1", description="automatically generated by tidbcloudy")\nprint(backup)\n\nconfig = CreateClusterConfig()\nconfig \\\n    .set_cluster_type("DEDICATED") \\\n    .set_cloud_provider("AWS") \\\n    .set_region("us-west-2") \\\n    .set_port(4399) \\\n    .set_root_password("your_root_password") \\\n    .set_component("tidb", "8C16G", 1) \\\n    .set_component("tikv", "8C32G", 3, 500) \\\n    .set_component("tiflash", "8C64G", 1, 500) \\\n    .add_current_ip_access()\nprint("Create a restore task from backup_id={}".format(backup_id))\nrestore = project.create_restore(backup_id=backup_id, name="restore-1", cluster_config=config)\nrestore_task = project.get_restore(restore.id)\nprint(restore_task.to_object())\nfor restore in project.iter_restores():\n    print(restore)\n```\n\n### Pause or resume your cluster\n\nTo pause or resume your cluster, run the [`6_pause_cluster.py`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples/6_pause_cluster.py).\n\n```python\nimport os\n\nimport tidbcloudy\nfrom tidbcloudy.api.specification import ClusterStatus\n\npublic_key = os.environ.get("PUBLIC_KEY")\nprivate_key = os.environ.get("PRIVATE_KEY")\nproject_id = "1234567890123456789"\ncluster_id = "1234567890123456789"\n\napi = tidbcloudy.TiDBCloud(public_key=public_key, private_key=private_key)\nproject = api.get_project(project_id, update_from_server=True)\ncluster = project.get_cluster(cluster_id)\n\nif cluster.status.cluster_status == ClusterStatus.AVAILABLE:\n    print("Pause the cluster id={}".format(cluster_id))\n    cluster.pause()\nif cluster.status.cluster_status == ClusterStatus.PAUSED:\n    print("Resume the cluster id={}".format(cluster_id))\n    cluster.resume()\nif cluster.status.cluster_status == ClusterStatus.RESUMING:\n    print("Wait for the RESUMING cluster id={} to be available".format(cluster_id))\n    cluster.wait_for_available()\n```\n\n### Delete all resources\n\n> Warning:\n>\n> This is a destructive operation. It will delete all resources in the project. **DO NOT** run this script in a production environment.\n\nTo delete all clusters and backup tasks in your project, run the [`7_delete_resources.py`](https://github.com/Oreoxmt/tidbcloudy/tree/main/examples/7_delete_resources.py).\n\n```python\nimport os\n\nimport tidbcloudy\nfrom tidbcloudy.api.specification import ClusterType\n\npublic_key = os.environ.get("PUBLIC_KEY")\nprivate_key = os.environ.get("PRIVATE_KEY")\nproject_id = "1234567890123456789"\n\napi = tidbcloudy.TiDBCloud(public_key=public_key, private_key=private_key)\nproject = api.get_project(project_id, update_from_server=True)\nfor cluster in project.iter_clusters():\n    print(cluster)\n    if cluster.cluster_type == ClusterType.DEDICATED:\n        for backup in cluster.iter_backups():\n            print(backup)\n            backup.delete()\n    cluster.delete()\n```\n\n## Related Projects\n\n- Go SDK: [go-tidbcloud-sdk-v1](https://github.com/c4pt0r/go-tidbcloud-sdk-v1) by [@c4pt0r](https://github.com/c4pt0r)\n- TiDB Cloud CLI: [OhMyTiUP/tidb-cloud](https://github.com/luyomo/OhMyTiUP/tree/main/pkg/tidbcloudapi) by [@luyomo](https://github.com/luyomo)\n- Official code samples in Go and Python: [tidbcloud-api-samples](https://github.com/tidbcloud/tidbcloud-api-samples)\n',
     'author': 'Aolin',
     'author_email': 'aolinz@outlook.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
+    'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `tidbcloudy-1.1.0a1/PKG-INFO` & `tidbcloudy-1.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: tidbcloudy
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: Python SDK for TiDB Cloud
 Author: Aolin
 Author-email: aolinz@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: mysqlclient (>=2.1.1,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
```


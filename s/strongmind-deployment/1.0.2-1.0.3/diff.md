# Comparing `tmp/strongmind_deployment-1.0.2-py3-none-any.whl.zip` & `tmp/strongmind_deployment-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6635 bytes, number of entries: 8
+Zip file size: 7177 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
--rw-r--r--  2.0 unx     5465 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
+-rw-r--r--  2.0 unx     9253 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
+-rw-r--r--  2.0 unx     7116 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
 -rw-r--r--  2.0 unx     1126 b- defN 20-Feb-02 00:00 strongmind_deployment/redis.py
-?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      710 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.2.dist-info/RECORD
-8 files, 17271 bytes uncompressed, 5377 bytes compressed:  68.9%
+?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      710 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.3.dist-info/RECORD
+8 files, 20020 bytes uncompressed, 5919 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: strongmind_deployment/rails.py
 Comment: 
 
 Filename: strongmind_deployment/redis.py
 Comment: 
 
-Filename: strongmind_deployment-1.0.2.dist-info/METADATA
+Filename: strongmind_deployment-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-1.0.2.dist-info/WHEEL
+Filename: strongmind_deployment-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-1.0.2.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-1.0.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-1.0.2.dist-info/RECORD
+Filename: strongmind_deployment-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/container.py

```diff
@@ -9,45 +9,114 @@
 from pulumi_cloudflare import get_zone, Record
 
 
 class ContainerComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:container', name, None, opts)
 
+        self.target_group = None
+        self.load_balancer_listener_redirect_http_to_https = None
+        self.load_balancer_listener = None
+        self.load_balancer = None
         self.cert_validation_cert = None
         self.cert_validation_record = None
         self.cert = None
         self._security_group_name = None
         self.cname_record = None
+        self.need_load_balancer = kwargs.get('need_load_balancer', True)
         self.container_image = kwargs.get('container_image')
-        self.app_path = kwargs.get('app_path') or './'
-        self.container_port = kwargs.get('container_port') or 3000
-        self.cpu = kwargs.get('cpu') or 256
-        self.memory = kwargs.get("memory") or 512
+        self.app_path = kwargs.get('app_path', './')
+        self.container_port = kwargs.get('container_port', 3000)
+        self.cpu = kwargs.get('cpu', 256)
+        self.memory = kwargs.get("memory", 512)
+        self.entry_point = kwargs.get('entry_point')
         self.env_vars = kwargs.get('env_vars', {})
         self.kwargs = kwargs
         self.env_name = os.environ.get('ENVIRONMENT_NAME', 'stage')
 
         stack = pulumi.get_stack()
         project = pulumi.get_project()
         project_stack = f"{project}-{stack}"
+        if name != 'container':
+            project_stack = f"{project_stack}-{name}"
 
         self.tags = {
             "product": project,
             "repository": project,
             "service": project,
             "environment": self.env_name,
         }
 
-        self.ecs_cluster = aws.ecs.Cluster("cluster",
-                                           name=project_stack,
-                                           tags=self.tags,
-                                           opts=pulumi.ResourceOptions(parent=self),
-                                           )
+        self.ecs_cluster_arn = kwargs.get('ecs_cluster_arn')
+        if self.ecs_cluster_arn is None:
+            self.ecs_cluster = aws.ecs.Cluster("cluster",
+                                               name=project_stack,
+                                               tags=self.tags,
+                                               opts=pulumi.ResourceOptions(parent=self),
+                                               )
+            self.ecs_cluster_arn = self.ecs_cluster.arn
+
+        if self.need_load_balancer:
+            self.setup_load_balancer(kwargs, project, project_stack)
+
+        log_name = 'log'
+        if name != 'container':
+            log_name = f'{name}-log'
+        logs = aws.cloudwatch.LogGroup(
+            log_name,
+            retention_in_days=14,
+            name=f'/aws/ecs/{project_stack}',
+            tags=self.tags
+        )
+        port_mappings = None
+        if self.target_group is not None:
+            port_mappings = [awsx.ecs.TaskDefinitionPortMappingArgs(
+                    container_port=self.container_port,
+                    host_port=self.container_port,
+                    target_group=self.target_group,
+                )]
+        task_definition_args = awsx.ecs.FargateServiceTaskDefinitionArgs(
+            skip_destroy=True,
+            family=project_stack,
+            container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
+                name=project_stack,
+                log_configuration=awsx.ecs.TaskDefinitionLogConfigurationArgs(
+                    log_driver="awslogs",
+                    options={
+                        "awslogs-group": logs.name,
+                        "awslogs-region": "us-west-2",
+                        "awslogs-stream-prefix": "container",
+                    },
+                ),
+                image=self.container_image,
+                cpu=self.cpu,
+                memory=self.memory,
+                entry_point=self.entry_point,
+                essential=True,
+                port_mappings=port_mappings,
+                environment=[{"name": k, "value": v} for k, v in self.env_vars.items()]
+            )
+        )
+        service_name = 'service'
+        if name != 'container':
+            service_name = f'{name}-service'
+        self.fargate_service = awsx.ecs.FargateService(
+            service_name,
+            name=project_stack,
+            cluster=self.ecs_cluster_arn,
+            continue_before_steady_state=True,
+            assign_public_ip=True,
+            task_definition_args=task_definition_args,
+            tags=self.tags,
+            opts=pulumi.ResourceOptions(parent=self),
+        )
 
+        self.register_outputs({})
+
+    def setup_load_balancer(self, kwargs, project, project_stack):
         default_vpc = awsx.ec2.DefaultVpc("default_vpc")
 
         self.target_group = aws.lb.TargetGroup(
             "targetgroup",
             name=project_stack,
             port=self.container_port,
             protocol="HTTP",
@@ -61,24 +130,23 @@
                 matcher="200",
                 interval=30,
                 timeout=5,
                 healthy_threshold=5,
                 unhealthy_threshold=2,
             ),
         )
+
         self.load_balancer = awsx.lb.ApplicationLoadBalancer(
             "loadbalancer",
             name=project_stack,
             default_target_group_port=self.container_port,
             tags=self.tags,
             opts=pulumi.ResourceOptions(parent=self),
         )
-
         self.dns(project)
-
         load_balancer_arn = kwargs.get('load_balancer_arn', self.load_balancer.load_balancer.arn)
         target_group_arn = kwargs.get('target_group_arn', self.target_group.arn)
         self.load_balancer_listener = aws.lb.Listener(
             "listener443",
             load_balancer_arn=load_balancer_arn,
             certificate_arn=self.cert.arn,
             port=443,
@@ -109,58 +177,14 @@
                     status_code="HTTP_301",
                 ),
             )],
             tags=self.tags,
             opts=pulumi.ResourceOptions(parent=self),
         )
 
-        logs = aws.cloudwatch.LogGroup(
-            f'log',
-            retention_in_days=14,
-            name=f'/aws/ecs/{project_stack}',
-            tags=self.tags
-        )
-        task_definition_args = awsx.ecs.FargateServiceTaskDefinitionArgs(
-            skip_destroy=True,
-            family=project_stack,
-            container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
-                name=project_stack,
-                log_configuration=awsx.ecs.TaskDefinitionLogConfigurationArgs(
-                    log_driver="awslogs",
-                    options={
-                        "awslogs-group": logs.name,
-                        "awslogs-region": "us-west-2",
-                        "awslogs-stream-prefix": "container",
-                    },
-                ),
-                image=self.container_image,
-                cpu=self.cpu,
-                memory=self.memory,
-                essential=True,
-                port_mappings=[awsx.ecs.TaskDefinitionPortMappingArgs(
-                    container_port=self.container_port,
-                    host_port=self.container_port,
-                    target_group=self.target_group,
-                )],
-                environment=[{"name": k, "value": v} for k, v in self.env_vars.items()]
-            )
-        )
-        self.fargate_service = awsx.ecs.FargateService(
-            "service",
-            name=project_stack,
-            cluster=self.ecs_cluster.arn,
-            continue_before_steady_state=True,
-            assign_public_ip=True,
-            task_definition_args=task_definition_args,
-            tags=self.tags,
-            opts=pulumi.ResourceOptions(parent=self),
-        )
-
-        self.register_outputs({})
-
     def dns(self, name):
         if self.env_name != "prod":
             name = f"{self.env_name}-{name}"
         domain = 'strongmind.com'
         full_name = f"{name}.{domain}"
         zone_id = self.kwargs.get('zone_id', 'b4b7fec0d0aacbd55c5a259d1e64fff5')
         lb_dns_name = self.kwargs.get('load_balancer_dns_name',
```

## strongmind_deployment/rails.py

```diff
@@ -9,18 +9,20 @@
 from strongmind_deployment.container import ContainerComponent
 from strongmind_deployment.redis import RedisComponent
 
 
 class RailsComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:rails', name, None, opts)
+        self.need_worker = None
         self.cname_record = None
         self.firewall_rule = None
         self.db_password = None
-        self.container = None
+        self.web_container = None
+        self.worker_container = None
         self.rds_serverless_cluster_instance = None
         self.rds_serverless_cluster = None
         self.kwargs = kwargs
         self.env_vars = self.kwargs.get('env_vars', {})
 
         self.env_name = os.environ.get('ENVIRONMENT_NAME', 'stage')
 
@@ -46,27 +48,27 @@
         self.security()
 
         self.register_outputs({})
 
     def security(self):
         container_security_group_id = self.kwargs.get(
             'container_security_group_id',
-            self.container.fargate_service.service.network_configuration.security_groups[0])  # pragma: no cover
+            self.web_container.fargate_service.service.network_configuration.security_groups[0])  # pragma: no cover
 
         self.firewall_rule = aws.ec2.SecurityGroupRule(
             'rds_security_group_rule',
             type='ingress',
             from_port=5432,
             to_port=5432,
             protocol='tcp',
             security_group_id=self.rds_serverless_cluster.vpc_security_group_ids[0],
             source_security_group_id=container_security_group_id,
             opts=pulumi.ResourceOptions(parent=self,
                                         depends_on=[self.rds_serverless_cluster_instance,
-                                                    self.container])
+                                                    self.web_container])
         )
 
     def ecs(self):
         container_image = os.environ['CONTAINER_IMAGE']
         master_key = os.environ['RAILS_MASTER_KEY']
         additional_env_vars = {
             'RAILS_MASTER_KEY': master_key,
@@ -78,18 +80,46 @@
             'RAILS_ENV': 'production'
         }
 
         self.env_vars.update(additional_env_vars)
         self.kwargs['env_vars'] = self.env_vars
         self.kwargs['container_image'] = container_image
 
-        self.container = ContainerComponent("container",
-                                            pulumi.ResourceOptions(parent=self),
-                                            **self.kwargs
-                                            )
+        web_entry_point = self.kwargs.get('web_entry_point', ["sh", "-c",
+                                                              "rails db:prepare db:migrate db:seed && "
+                                                              "rails assets:precompile && "
+                                                              "rails server --port 3000 -b 0.0.0.0"])
+
+        self.kwargs['entry_point'] = web_entry_point
+
+        self.web_container = ContainerComponent("container",
+                                                pulumi.ResourceOptions(parent=self),
+                                                **self.kwargs
+                                                )
+
+        self.need_worker = self.kwargs.get('need_worker', None)
+        if self.need_worker is None:
+            # If we don't know if we need a worker, check for sidekiq in the Gemfile
+            self.need_worker = os.path.exists('../Gemfile') and 'sidekiq' in open('../Gemfile').read()
+
+        if self.need_worker:
+            self.setup_worker()
+
+    def setup_worker(self):
+        worker_entry_point = self.kwargs.get('worker_entry_point', ["sh", "-c", "bundle exec sidekiq"])
+        self.kwargs['entry_point'] = worker_entry_point
+        self.kwargs['cpu'] = self.kwargs.get('worker_cpu')
+        self.kwargs['memory'] = self.kwargs.get('worker_memory')
+        self.kwargs['app_path'] = self.kwargs.get('worker_app_path')
+        self.kwargs['need_load_balancer'] = False
+        self.kwargs['ecs_cluster_arn'] = self.web_container.ecs_cluster_arn
+        self.worker_container = ContainerComponent("worker",
+                                                   pulumi.ResourceOptions(parent=self),
+                                                   **self.kwargs
+                                                   )
 
     def rds(self, project_stack):
         self.db_password = random.RandomPassword("password",
                                                  length=30,
                                                  special=False)
         self.rds_serverless_cluster = aws.rds.Cluster(
             'rds_serverless_cluster',
```

## Comparing `strongmind_deployment-1.0.2.dist-info/METADATA` & `strongmind_deployment-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 1.0.2
+Version: 1.0.3
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-1.0.2.dist-info/licenses/LICENSE` & `strongmind_deployment-1.0.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `strongmind_deployment-1.0.2.dist-info/RECORD` & `strongmind_deployment-1.0.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 strongmind_deployment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-strongmind_deployment/container.py,sha256=xLJ8rpouHE_WBhcg4TcBgMos5FkdSrQ-3nu05iD-DHM,8155
-strongmind_deployment/rails.py,sha256=PgyH4aDeHnFsnUQN7OnJdxbPZemeYcUFWevQQcq3NZg,5465
+strongmind_deployment/container.py,sha256=9La_hbQkzof46-IaBG7sdWXVr9wxCns15GXfxAg4WAQ,9253
+strongmind_deployment/rails.py,sha256=FSUHNG2j7_0EFnSgJUN9_ZBsFaiEq7dQ_zBUIzpyvg8,7116
 strongmind_deployment/redis.py,sha256=pYiSCRBQtO9TU69KVt0GrmJyB_GhGEz_hQUucw9vBUA,1126
-strongmind_deployment-1.0.2.dist-info/METADATA,sha256=8jdQPKNVX3S1mEWUtvDhGuibqQa70Fo8f4KTEVF6EN0,675
-strongmind_deployment-1.0.2.dist-info/WHEEL,sha256=y1bSCq4r5i4nMmpXeUJMqs3ipKvkZObrIXSvJHm1qCI,87
-strongmind_deployment-1.0.2.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
-strongmind_deployment-1.0.2.dist-info/RECORD,,
+strongmind_deployment-1.0.3.dist-info/METADATA,sha256=rz14hlUPnR7CVuENaFcBg8fYo4pRJ62sYJCg6Ip_tHM,675
+strongmind_deployment-1.0.3.dist-info/WHEEL,sha256=y1bSCq4r5i4nMmpXeUJMqs3ipKvkZObrIXSvJHm1qCI,87
+strongmind_deployment-1.0.3.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
+strongmind_deployment-1.0.3.dist-info/RECORD,,
```


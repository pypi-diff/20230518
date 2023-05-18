# Comparing `tmp/sym_flow_cli-7.4.0.tar.gz` & `tmp/sym_flow_cli-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym_flow_cli-7.4.0.tar", max compression
+gzip compressed data, was "sym_flow_cli-8.0.0.tar", max compression
```

## Comparing `sym_flow_cli-7.4.0.tar` & `sym_flow_cli-8.0.0.tar`

### file list

```diff
@@ -1,133 +1,139 @@
--rw-r--r--   0        0        0      160 2023-05-09 21:04:23.040356 sym_flow_cli-7.4.0/DESCRIPTION.md
--rw-r--r--   0        0        0     1790 2023-05-09 21:04:24.892361 sym_flow_cli-7.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/__init__.py
--rw-r--r--   0        0        0       60 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/__init__.py
--rw-r--r--   0        0        0     4711 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/README.md
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/connectors/__init__.py
--rw-r--r--   0        0        0      244 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/connectors/connectors.tf
--rw-r--r--   0        0        0      677 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/connectors/iam_connector.tf
--rw-r--r--   0        0        0     1664 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/connectors/sso_connector.tf
--rw-r--r--   0        0        0     1268 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/environment.tf
--rw-r--r--   0        0        0     1375 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/environment_with_runtime.tf
--rw-r--r--   0        0        0     3596 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/runtime.tf
--rw-r--r--   0        0        0      637 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/runtime_sso_assume_roles.tf
--rw-r--r--   0        0        0     1484 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/secrets.tf
--rw-r--r--   0        0        0      370 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/sym_runtime.tf
--rw-r--r--   0        0        0      115 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/versions.tf
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/__init__.py
--rw-r--r--   0        0        0     1494 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/approval_impl.txt
--rw-r--r--   0        0        0      928 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/approval_only.tf
--rw-r--r--   0        0        0     2979 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_iam.tf
--rw-r--r--   0        0        0     4190 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_lambda.tf
--rw-r--r--   0        0        0     2076 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_sso.tf
--rw-r--r--   0        0        0     1188 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_sso_group_target.tf
--rw-r--r--   0        0        0     1052 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_sso_permission_set_target.tf
--rw-r--r--   0        0        0      450 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/impl.txt
--rw-r--r--   0        0        0     1777 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/lambda_handler.txt
--rw-r--r--   0        0        0     1250 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/lambda_impl.txt
--rw-r--r--   0        0        0     3983 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/okta.tf
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/__init__.py
--rw-r--r--   0        0        0       84 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/__init__.py
--rw-r--r--   0        0        0      775 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/bots.py
--rw-r--r--   0        0        0     1762 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/create.py
--rw-r--r--   0        0        0     1444 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/delete.py
--rw-r--r--   0        0        0     1607 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/delete_identity.py
--rw-r--r--   0        0        0     1922 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/list.py
--rw-r--r--   0        0        0     1665 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/update_identity.py
--rw-r--r--   0        0        0       46 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/config/__init__.py
--rw-r--r--   0        0        0      458 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/config/config.py
--rw-r--r--   0        0        0     1027 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/config/config_get.py
--rw-r--r--   0        0        0      560 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/docs.py
--rw-r--r--   0        0        0       93 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/domains/__init__.py
--rw-r--r--   0        0        0      565 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/domains/add.py
--rw-r--r--   0        0        0      936 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/domains/domains.py
--rw-r--r--   0        0        0     1180 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/domains/list.py
--rw-r--r--   0        0        0      658 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/domains/remove.py
--rw-r--r--   0        0        0     7248 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/generate.py
--rw-r--r--   0        0        0     5120 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/init.py
--rw-r--r--   0        0        0     2110 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/login.py
--rw-r--r--   0        0        0       72 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/organization/__init__.py
--rw-r--r--   0        0        0      434 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/organization/organization.py
--rw-r--r--   0        0        0     1635 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/organization/organization_configure_mfa.py
--rw-r--r--   0        0        0       99 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/resources/__init__.py
--rw-r--r--   0        0        0     2316 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/resources/list.py
--rw-r--r--   0        0        0      640 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/resources/resources.py
--rw-r--r--   0        0        0       60 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/__init__.py
--rw-r--r--   0        0        0      551 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/click/external_id_option.py
--rw-r--r--   0        0        0      805 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/click/inquirer_choice.py
--rw-r--r--   0        0        0     1058 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/click/service_type_choice.py
--rw-r--r--   0        0        0      728 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/click/service_type_option.py
--rw-r--r--   0        0        0      570 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/hooks/slack_delete.py
--rw-r--r--   0        0        0      626 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/services.py
--rw-r--r--   0        0        0     2221 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/services_delete.py
--rw-r--r--   0        0        0      947 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/services_list.py
--rw-r--r--   0        0        0     1081 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/services/services_update.py
--rw-r--r--   0        0        0     3845 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/status.py
--rw-r--r--   0        0        0     2708 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/symflow.py
--rw-r--r--   0        0        0       90 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/tokens/__init__.py
--rw-r--r--   0        0        0     2563 2023-05-09 21:04:23.044356 sym_flow_cli-7.4.0/sym/flow/cli/commands/tokens/issue.py
--rw-r--r--   0        0        0     1711 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/tokens/list.py
--rw-r--r--   0        0        0      589 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/tokens/revoke.py
--rw-r--r--   0        0        0      564 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/tokens/tokens.py
--rw-r--r--   0        0        0       87 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/__init__.py
--rw-r--r--   0        0        0     4428 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/create.py
--rw-r--r--   0        0        0     1471 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/delete.py
--rw-r--r--   0        0        0     1614 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/delete_identity.py
--rw-r--r--   0        0        0     1207 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/list.py
--rw-r--r--   0        0        0     1503 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/list_identities.py
--rw-r--r--   0        0        0     1289 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/set_role.py
--rw-r--r--   0        0        0     3561 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/update.py
--rw-r--r--   0        0        0     1652 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/update_identity.py
--rw-r--r--   0        0        0     1501 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/update_name.py
--rw-r--r--   0        0        0     1177 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/users.py
--rw-r--r--   0        0        0     1448 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/users/utils.py
--rw-r--r--   0        0        0      297 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/commands/version.py
--rw-r--r--   0        0        0     7211 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/errors.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/__init__.py
--rw-r--r--   0        0        0    10200 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/api.py
--rw-r--r--   0        0        0     5196 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/api_operations.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/__init__.py
--rw-r--r--   0        0        0     1300 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/approval_only.py
--rw-r--r--   0        0        0     6125 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/aws.py
--rw-r--r--   0        0        0     2986 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/aws_iam.py
--rw-r--r--   0        0        0     2712 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/aws_lambda.py
--rw-r--r--   0        0        0     7331 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/aws_sso.py
--rw-r--r--   0        0        0     9471 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/core.py
--rw-r--r--   0        0        0     3369 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/okta.py
--rw-r--r--   0        0        0       39 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/config/__init__.py
--rw-r--r--   0        0        0     5992 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/config/config.py
--rw-r--r--   0        0        0     1929 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/config/lock.py
--rw-r--r--   0        0        0     1923 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/config/thread_safe_file.py
--rw-r--r--   0        0        0      507 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/constants.py
--rw-r--r--   0        0        0     2489 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/global_options.py
--rw-r--r--   0        0        0     2378 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/identity_operations.py
--rw-r--r--   0        0        0     1469 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/jwt.py
--rw-r--r--   0        0        0        0 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/login/__init__.py
--rw-r--r--   0        0        0     8826 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/login/handler.py
--rw-r--r--   0        0        0     3986 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/login/login_flow.py
--rw-r--r--   0        0        0     1446 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/output.py
--rw-r--r--   0        0        0     1336 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/profile_operations.py
--rw-r--r--   0        0        0     4933 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/rest.py
--rw-r--r--   0        0        0     2426 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/sentry.py
--rw-r--r--   0        0        0     3192 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/terraform.py
--rw-r--r--   0        0        0     2267 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/tracked_command.py
--rw-r--r--   0        0        0     6681 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/users.py
--rw-r--r--   0        0        0     1212 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/utils.py
--rw-r--r--   0        0        0     1972 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/version.py
--rw-r--r--   0        0        0      412 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/helpers/yaml.py
--rw-r--r--   0        0        0      192 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/models/__init__.py
--rw-r--r--   0        0        0      123 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/models/auth.py
--rw-r--r--   0        0        0      206 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/models/organization.py
--rw-r--r--   0        0        0     1105 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/models/resource.py
--rw-r--r--   0        0        0      372 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/models/service.py
--rw-r--r--   0        0        0     3090 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/models/service_type.py
--rw-r--r--   0        0        0      705 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/models/token.py
--rw-r--r--   0        0        0     4814 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/models/user.py
--rw-r--r--   0        0        0      286 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/models/user_type.py
--rw-r--r--   0        0        0      171 2023-05-09 21:04:23.048356 sym_flow_cli-7.4.0/sym/flow/cli/symflow.py
--rw-r--r--   0        0        0       22 2023-05-09 21:04:24.944361 sym_flow_cli-7.4.0/sym/flow/cli/version.py
--rw-r--r--   0        0        0     2045 1970-01-01 00:00:00.000000 sym_flow_cli-7.4.0/setup.py
--rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 sym_flow_cli-7.4.0/PKG-INFO
+-rw-r--r--   0        0        0      160 2023-05-18 14:32:36.761746 sym_flow_cli-8.0.0/DESCRIPTION.md
+-rw-r--r--   0        0        0     1790 2023-05-18 14:32:38.493768 sym_flow_cli-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/__init__.py
+-rw-r--r--   0        0        0     4711 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/connectors/__init__.py
+-rw-r--r--   0        0        0      350 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/connectors/connectors.tf
+-rw-r--r--   0        0        0      689 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/connectors/iam_connector.tf
+-rw-r--r--   0        0        0      315 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/connectors/runtime_connector.tf
+-rw-r--r--   0        0        0      467 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/connectors/runtime_connector_with_account_id_safelist.tf
+-rw-r--r--   0        0        0     1676 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/connectors/sso_connector.tf
+-rw-r--r--   0        0        0     1268 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/environment.tf
+-rw-r--r--   0        0        0      232 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/environment_with_runtime.tf
+-rw-r--r--   0        0        0     1142 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/secrets.tf
+-rw-r--r--   0        0        0      115 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/versions.tf
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/__init__.py
+-rw-r--r--   0        0        0     1494 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/approval_impl.txt
+-rw-r--r--   0        0        0      910 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/approval_only.tf
+-rw-r--r--   0        0        0     2985 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_iam.tf
+-rw-r--r--   0        0        0     4187 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_lambda.tf
+-rw-r--r--   0        0        0     2082 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_sso.tf
+-rw-r--r--   0        0        0     1189 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_sso_group_target.tf
+-rw-r--r--   0        0        0     1052 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_sso_permission_set_target.tf
+-rw-r--r--   0        0        0      450 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/impl.txt
+-rw-r--r--   0        0        0     1777 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/lambda_handler.txt
+-rw-r--r--   0        0        0     1250 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/lambda_impl.txt
+-rw-r--r--   0        0        0     4025 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/okta.tf
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/migration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/migration/v8/__init__.py
+-rw-r--r--   0        0        0      679 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/migration/v8/migration_v8.tf
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/__init__.py
+-rw-r--r--   0        0        0      775 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/bots.py
+-rw-r--r--   0        0        0     1762 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/create.py
+-rw-r--r--   0        0        0     1444 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/delete.py
+-rw-r--r--   0        0        0     1607 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/delete_identity.py
+-rw-r--r--   0        0        0     1922 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/list.py
+-rw-r--r--   0        0        0     1665 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/update_identity.py
+-rw-r--r--   0        0        0       46 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/config/__init__.py
+-rw-r--r--   0        0        0      458 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/config/config.py
+-rw-r--r--   0        0        0     1027 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/config/config_get.py
+-rw-r--r--   0        0        0      560 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/docs.py
+-rw-r--r--   0        0        0       93 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/domains/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/domains/add.py
+-rw-r--r--   0        0        0      936 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/domains/domains.py
+-rw-r--r--   0        0        0     1180 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/domains/list.py
+-rw-r--r--   0        0        0      658 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/domains/remove.py
+-rw-r--r--   0        0        0     9432 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/generate.py
+-rw-r--r--   0        0        0     5120 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/init.py
+-rw-r--r--   0        0        0     2110 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/login.py
+-rw-r--r--   0        0        0     4578 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/migrate.py
+-rw-r--r--   0        0        0       72 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/organization/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/organization/organization.py
+-rw-r--r--   0        0        0     1635 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/organization/organization_configure_mfa.py
+-rw-r--r--   0        0        0       99 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/resources/__init__.py
+-rw-r--r--   0        0        0     2316 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/resources/list.py
+-rw-r--r--   0        0        0      640 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/resources/resources.py
+-rw-r--r--   0        0        0       60 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/__init__.py
+-rw-r--r--   0        0        0      551 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/click/external_id_option.py
+-rw-r--r--   0        0        0      805 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/click/inquirer_choice.py
+-rw-r--r--   0        0        0     1058 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/click/service_type_choice.py
+-rw-r--r--   0        0        0      728 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/click/service_type_option.py
+-rw-r--r--   0        0        0      570 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/hooks/slack_delete.py
+-rw-r--r--   0        0        0      626 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/services.py
+-rw-r--r--   0        0        0     2221 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/services_delete.py
+-rw-r--r--   0        0        0      947 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/services_list.py
+-rw-r--r--   0        0        0     1081 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/services/services_update.py
+-rw-r--r--   0        0        0     3845 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/status.py
+-rw-r--r--   0        0        0     2802 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/symflow.py
+-rw-r--r--   0        0        0       90 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/tokens/__init__.py
+-rw-r--r--   0        0        0     2563 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/tokens/issue.py
+-rw-r--r--   0        0        0     1711 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/tokens/list.py
+-rw-r--r--   0        0        0      589 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/tokens/revoke.py
+-rw-r--r--   0        0        0      564 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/tokens/tokens.py
+-rw-r--r--   0        0        0       87 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/__init__.py
+-rw-r--r--   0        0        0     4428 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/create.py
+-rw-r--r--   0        0        0     1471 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/delete.py
+-rw-r--r--   0        0        0     1614 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/delete_identity.py
+-rw-r--r--   0        0        0     1207 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/list.py
+-rw-r--r--   0        0        0     1503 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/list_identities.py
+-rw-r--r--   0        0        0     1289 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/set_role.py
+-rw-r--r--   0        0        0     3561 2023-05-18 14:32:36.765746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/update.py
+-rw-r--r--   0        0        0     1652 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/update_identity.py
+-rw-r--r--   0        0        0     1501 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/update_name.py
+-rw-r--r--   0        0        0     1177 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/users.py
+-rw-r--r--   0        0        0     1448 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/commands/users/utils.py
+-rw-r--r--   0        0        0      297 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/commands/version.py
+-rw-r--r--   0        0        0     7211 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/errors.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/__init__.py
+-rw-r--r--   0        0        0    10200 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/api.py
+-rw-r--r--   0        0        0     5196 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/api_operations.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/__init__.py
+-rw-r--r--   0        0        0     1300 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/approval_only.py
+-rw-r--r--   0        0        0     3812 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/aws.py
+-rw-r--r--   0        0        0     2978 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/aws_iam.py
+-rw-r--r--   0        0        0     2704 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/aws_lambda.py
+-rw-r--r--   0        0        0     9082 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/aws_sso.py
+-rw-r--r--   0        0        0    10792 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/core.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/migration/__init__.py
+-rw-r--r--   0        0        0    20711 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/migration/migrate.py
+-rw-r--r--   0        0        0      460 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/migration/moved_block.py
+-rw-r--r--   0        0        0     3392 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/okta.py
+-rw-r--r--   0        0        0       39 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/config/__init__.py
+-rw-r--r--   0        0        0     5992 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/config/config.py
+-rw-r--r--   0        0        0     1929 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/config/lock.py
+-rw-r--r--   0        0        0     1923 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/config/thread_safe_file.py
+-rw-r--r--   0        0        0      507 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/constants.py
+-rw-r--r--   0        0        0     2178 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/global_options.py
+-rw-r--r--   0        0        0     2378 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/identity_operations.py
+-rw-r--r--   0        0        0     1469 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/jwt.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/login/__init__.py
+-rw-r--r--   0        0        0     8826 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/login/handler.py
+-rw-r--r--   0        0        0     3986 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/login/login_flow.py
+-rw-r--r--   0        0        0     1446 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/output.py
+-rw-r--r--   0        0        0     1336 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/profile_operations.py
+-rw-r--r--   0        0        0     4933 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/rest.py
+-rw-r--r--   0        0        0     2426 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/sentry.py
+-rw-r--r--   0        0        0     4102 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/terraform.py
+-rw-r--r--   0        0        0     2267 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/tracked_command.py
+-rw-r--r--   0        0        0     6681 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/users.py
+-rw-r--r--   0        0        0     1212 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/utils.py
+-rw-r--r--   0        0        0     1972 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/version.py
+-rw-r--r--   0        0        0      412 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/helpers/yaml.py
+-rw-r--r--   0        0        0      192 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/models/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/models/auth.py
+-rw-r--r--   0        0        0      206 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/models/organization.py
+-rw-r--r--   0        0        0     1105 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/models/resource.py
+-rw-r--r--   0        0        0      372 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/models/service.py
+-rw-r--r--   0        0        0     3090 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/models/service_type.py
+-rw-r--r--   0        0        0      705 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/models/token.py
+-rw-r--r--   0        0        0     4814 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/models/user.py
+-rw-r--r--   0        0        0      286 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/models/user_type.py
+-rw-r--r--   0        0        0      171 2023-05-18 14:32:36.769746 sym_flow_cli-8.0.0/sym/flow/cli/symflow.py
+-rw-r--r--   0        0        0       22 2023-05-18 14:32:38.537769 sym_flow_cli-8.0.0/sym/flow/cli/version.py
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 sym_flow_cli-8.0.0/setup.py
+-rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 sym_flow_cli-8.0.0/PKG-INFO
```

### Comparing `sym_flow_cli-7.4.0/pyproject.toml` & `sym_flow_cli-8.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sym-flow-cli"
-version = "7.4.0"
+version = "8.0.0"
 description = "Sym's Official CLI for Implementers"
 authors = ["SymOps, Inc. <pypi@symops.io>"]
 packages = [{ include = "sym" }]
 readme = "DESCRIPTION.md"
 homepage = "https://symops.com/"
 documentation = "https://docs.symops.com/docs/install-sym-flow-cli"
 classifiers = [
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/README.md` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/README.md`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/connectors/iam_connector.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/connectors/iam_connector.tf`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ############ AWS IAM Connector Setup ##############
 # The iam_connector module creates a new IAM Role with the permissions to add and remove users from IAM Groups.
 module "iam_connector" {
   source  = "symopsio/iam-connector/aws"
   version = ">= 1.0.0"
 
   environment       = local.environment_name
-  runtime_role_arns = [aws_iam_role.sym_runtime_connector_role.arn]
+  runtime_role_arns = [module.runtime_connector.sym_runtime_connector_role.arn]
 }
 
 # The Integration your Strategy uses to manage IAM Groups
 resource "sym_integration" "aws_iam_context" {
   type        = "permission_context"
   name        = "${local.environment_name}-aws-iam-context"
   external_id = module.iam_connector.settings.account_id
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/connectors/sso_connector.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/connectors/sso_connector.tf`

 * *Files 15% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   # Provision the SSO connector in the AWS account where your AWS
   # SSO instance lives.
   providers = {
     aws = aws.sso
   }
 
   environment       = local.environment_name
-  runtime_role_arns = [aws_iam_role.sym_runtime_connector_role.arn]
+  runtime_role_arns = [module.runtime_connector.sym_runtime_connector_role.arn]
 }
 
 # The Integration your Strategy uses to manage SSO Permission Sets
 resource "sym_integration" "aws_sso_context" {
   type        = "permission_context"
   name        = "${local.environment_name}-aws-sso-context"
   external_id = one(data.aws_ssoadmin_instances.this.arns)
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/environment.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/environment.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/core/secrets.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/core/secrets.tf`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,25 @@
 # This file was generated by symflow CLI vSYM_TEMPLATE_VAR_SYMFLOW_VERSION on SYM_TEMPLATE_VAR_GENERATION_TIME UTC.
 # EDIT AT YOUR OWN RISK. If the resources in this file change, subsequent Flows added by `symflow generate` may not work as-is.
 
+# This secrets_manager_access module defines an AWS IAM Policy and attachment that grants the Sym Runtime Role
+# the permissions to read secrets from AWS Secrets Manager that are under the /sym/ path and tagged with
+# `SymEnv = local.environment_name`.
+module "secrets_manager_access" {
+  source  = "symopsio/secretsmgr-addon/aws"
+  version = "~> 1.1"
 
-resource "aws_iam_policy" "secrets_manager_access" {
-  name = "SymSecretsManager${title(local.environment_name)}"
-  path = "/sym/"
-
-  description = "AWS IAM policy granting the Sym Runtime read-only permissions to Secrets Manager secrets tagged with `SymEnv = environment_name`."
-  policy      = <<EOT
-{
-  "Version": "2012-10-17",
-  "Statement": [
-    {
-      "Effect": "Allow",
-      "Action": [
-        "secretsmanager:DescribeSecret",
-        "secretsmanager:GetSecretValue"
-      ],
-      "Resource": "*",
-      "Condition": { "StringEquals": { "secretsmanager:ResourceTag/SymEnv": "${local.environment_name}" } }
-    }
-  ]
-}
-EOT
-}
-
-resource "aws_iam_role_policy_attachment" "attach_secrets_manager_access" {
-  policy_arn = aws_iam_policy.secrets_manager_access.arn
-  role       = aws_iam_role.sym_runtime_connector_role.name
+  environment   = local.environment_name
+  iam_role_name = module.runtime_connector.sym_runtime_connector_role.name
 }
 
 # This resource tells Sym how to access your AWS account's Secrets Manager instance.
 resource "sym_secrets" "this" {
   type = "aws_secrets_manager"
   name = "${local.environment_name}-sym-secrets"
 
   settings = {
-    # This tells Sym to use the runtime_context integration defined in runtime.tf to access
+    # This tells Sym to use the sym_integration defined in the runtime_connector module when accessing
     # your AWS account's Secrets Manager.
-    context_id = sym_integration.runtime_context.id
+    context_id = module.runtime_connector.sym_integration.id
   }
 }
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/approval_impl.txt` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/approval_impl.txt`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/approval_only.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/approval_only.tf`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Modify this file to customize approvals with Sym.
 
 
 resource "sym_flow" "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_approval" {
   name  = "SYM_TEMPLATE_VAR_FLOW_NAME-approval"
   label = "Approval-Only"
 
-  implementation = "${path.module}/impls/approval_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py"
+  implementation = file("${path.module}/impls/approval_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py")
   environment_id = sym_environment.this.id
 
   params {
     # The prompt_field block defines a custom form field for the Slack modal that
     # requesters fill out to make their requests.
     prompt_field {
-      name           = "resource-identifier"
-      label          = "What do you need access to?"
-      type           = "string"
-      required       = true
+      name     = "resource-identifier"
+      label    = "What do you need access to?"
+      type     = "string"
+      required = true
     }
 
     prompt_field {
       name     = "reason"
       label    = "Why do you need access?"
       type     = "string"
       required = true
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_iam.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_iam.tf`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 }
 
 
 resource "sym_flow" "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_aws_iam" {
   name  = "SYM_TEMPLATE_VAR_FLOW_NAME-aws-iam"
   label = "AWS IAM Group Access"
 
-  implementation = "${path.module}/impls/aws_iam_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py"
+  implementation = file("${path.module}/impls/aws_iam_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py")
   environment_id = sym_environment.this.id
 
   params {
     # By specifying a strategy, this Flow will now be able to manage access (escalate/de-escalate)
     # to the targets specified in the `sym_strategy` resource.
     strategy_id = sym_strategy.SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_aws_iam.id
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_lambda.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_lambda.tf`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 module "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_lambda_connector" {
   source  = "symopsio/lambda-connector/aws"
   version = ">= 1.0.0"
 
   environment = "SYM_TEMPLATE_VAR_FLOW_NAME"
   lambda_arns = [module.SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_lambda_function.lambda_function_arn]
 
-  # The aws_iam_role.sym_runtime_connector_role resource is defined in `runtime.tf`.
-  runtime_role_arns = [aws_iam_role.sym_runtime_connector_role.arn]
+  # The runtime_connector module is defined in `connectors.tf`.
+  runtime_role_arns = [module.runtime_connector.sym_runtime_connector_role.arn]
 }
 
 # This Integration provides your Strategy the permissions needed to invoke your AWS Lambda.
 # It points to to the AWS IAM resources created by the `SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_lambda_connector` module.
 resource "sym_integration" "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_lambda_context" {
   type = "permission_context"
   name = "SYM_TEMPLATE_VAR_FLOW_NAME-lambda-context"
@@ -65,15 +65,15 @@
   targets        = [sym_target.SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_lambda_function.id]
 }
 
 # A Sym Flow that executes an AWS Lambda on escalate and de-escalate Sym events.
 resource "sym_flow" "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_lambda" {
   name = "SYM_TEMPLATE_VAR_FLOW_NAME-lambda"
 
-  implementation = "${path.module}/impls/aws_lambda_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py"
+  implementation = file("${path.module}/impls/aws_lambda_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py")
 
   # The sym_environment resource is defined in `environment.tf`.
   environment_id = sym_environment.this.id
 
   params {
     # By specifying a strategy, this Flow will now be able to manage access (escalate/de-escalate)
     # to the Targets specified in the `sym_strategy` resource.
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_sso.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_sso.tf`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   }
 }
 
 resource "sym_flow" "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_aws_sso" {
   name  = "SYM_TEMPLATE_VAR_FLOW_NAME-aws-sso"
   label = "AWS SSO Access"
 
-  implementation = "${path.module}/impls/aws_sso_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py"
+  implementation = file("${path.module}/impls/aws_sso_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py")
   environment_id = sym_environment.this.id
 
   params {
     # By specifying a strategy, this Flow will now be able to manage access (escalate/de-escalate)
     # to the targets specified in the `sym_strategy` resource.
     strategy_id = sym_strategy.SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_aws_sso.id
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_sso_group_target.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_sso_group_target.tf`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       attribute_value = "SYM_TEMPLATE_VAR_SSO_GROUP_NAME"
     }
   }
 }
 
 # An AWS SSO Group target that your Sym Strategy can manage access to
 resource "sym_target" "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_sso_group_target" {
-  type = "aws_sso_group"
+  type  = "aws_sso_group"
   name  = "SYM_TEMPLATE_VAR_FLOW_NAME-sso-group"
   label = data.aws_identitystore_group.SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_SYM_TEMPLATE_VAR_SSO_GROUP_RESOURCE_NAME.display_name
 
   settings = {
     # `type=aws_sso_group` sym_targets have a required setting `group_id`,
     # which must be the AWS SSO Group ID the requester will be escalated to when this target is selected.
     group_id = data.aws_identitystore_group.SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_SYM_TEMPLATE_VAR_SSO_GROUP_RESOURCE_NAME.group_id
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/aws_sso_permission_set_target.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/aws_sso_permission_set_target.tf`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/lambda_handler.txt` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/lambda_handler.txt`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/lambda_impl.txt` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/lambda_impl.txt`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/code_generation_templates/flows/okta.tf` & `sym_flow_cli-8.0.0/sym/flow/cli/code_generation_templates/flows/okta.tf`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 # An AWS Secrets Manager Secret to hold your Okta API Key. Set the value with:
 # aws secretsmanager put-secret-value --secret-id "sym/SYM_TEMPLATE_VAR_FLOW_NAME/okta-api-key" --secret-string "YOUR-OKTA-API-KEY"
 resource "aws_secretsmanager_secret" "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_okta_api_key" {
   name        = "sym/SYM_TEMPLATE_VAR_FLOW_NAME/okta-api-key"
   description = "API Key for Sym to call Okta APIs"
 
   tags = {
-    # This SymEnv tag is required because the aws_iam_policy.secrets_manager_access from secrets.tf
-    # only grants access to secrets tagged with a matching SymEnv value
+    # This SymEnv tag is required because the secrets_manager_access module defined in secrets.tf
+    # only grants access to secrets tagged with a SymEnv value that matches its `environment` input variable.
     SymEnv = local.environment_name
   }
 }
 
 # This resource tells Sym how to access your Okta API Key.
 resource "sym_secret" "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_okta_api_key" {
   # The source of your secrets and the permissions needed to access
@@ -64,15 +64,15 @@
   targets = [sym_target.SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_okta_group.id]
 }
 
 resource "sym_flow" "SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_okta" {
   name  = "SYM_TEMPLATE_VAR_FLOW_NAME-okta"
   label = "Okta Group Access"
 
-  implementation = "${path.module}/impls/okta_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py"
+  implementation = file("${path.module}/impls/okta_SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_impl.py")
   environment_id = sym_environment.this.id
 
   params {
     # By specifying a strategy, this Flow will now be able to manage access (escalate/de-escalate)
     # to the targets specified in the `sym_strategy` resource.
     strategy_id = sym_strategy.SYM_TEMPLATE_VAR_FLOW_RESOURCE_NAME_okta.id
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/bots.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/bots.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/create.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/create.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/delete.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/delete.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/delete_identity.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/delete_identity.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/list.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/bots/update_identity.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/bots/update_identity.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/config/config_get.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/config/config_get.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/docs.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/docs.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/domains/add.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/domains/add.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/domains/domains.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/domains/domains.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/domains/list.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/domains/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/domains/remove.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/domains/remove.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/generate.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/generate.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from sym.flow.cli.helpers.code_generation.aws_sso import AWSSSOFlowGeneration
 from sym.flow.cli.helpers.code_generation.core import FlowGeneration, get_valid_slug
 from sym.flow.cli.helpers.code_generation.okta import OktaFlowGeneration
 from sym.flow.cli.helpers.config import Config
 from sym.flow.cli.helpers.global_options import GlobalOptions
 from sym.flow.cli.helpers.tracked_command import TrackedCommand
 from sym.flow.cli.helpers.utils import get_or_prompt
+from sym.flow.cli.helpers.version import get_current_version
 
 FLOW_TYPE_OPTIONS = ["okta", "approval-only", "aws-iam", "aws-lambda", "aws-sso"]
 
 
 @click.command(cls=TrackedCommand, short_help="Generate Terraform to configure a Sym Flow.")
 @click.make_pass_decorator(GlobalOptions, ensure=True)
 @click.option(
@@ -49,14 +50,18 @@
     directory_placeholder = "the current directory" if directory == "." else "the directory `" + directory + "`"
     if not Path(f"{directory}/environment.tf").is_file() or not Path(f"{directory}/versions.tf").is_file():
         cli_output.fail(
             "This command must be run inside a directory created by `symflow init`. Please run that command first.",
             hint=f"Hint: {directory_placeholder.capitalize()} must have `environment.tf` and `versions.tf` files.",
         )
 
+    # Check if any files were generated by a previous major version. If so, warn the user and confirm if they wish to
+    # proceed anyway.
+    check_file_compatibility(directory)
+
     cli_output.info(
         f"\nWelcome to Sym! This command will generate new files required to configure a Sym Flow in {directory_placeholder}.\n",
     )
 
     if not type_:
         # If they passed in a type_, then we don't need to print this hint
         cli_output.warn(
@@ -133,14 +138,48 @@
     generator.final_instructions()
 
     cli_output.info(f"\nAfter everything is configured:")
     cli_output.actionable(f"Run /sym in Slack")
     cli_output.info(f"... to see your new Flow in action!")
 
 
+def check_file_compatibility(directory: str):
+    """
+    In all the existing Terraform files, check if they were generated by a previous symflow major version.
+    If so, warn the user that the new files will be incompatible and tell them to either manually migrate or
+    attempt `symflow migrate`.
+
+    Displays a confirm prompt to ask if the user wishes to proceed anyway, where the default is No.
+
+    Args:
+        directory: The directory in which to generate files
+    """
+    existing_tf_files = Path(directory).glob("*.tf")
+
+    # For now, we only have v7 and v8, so we only need to check for v7 files (current version is v8).
+    # In the future, we might need to consider keeping track of which major versions are code-gen compatible instead.
+    for file_path in existing_tf_files:
+        with open(file_path, "r") as file:
+            if "symflow CLI v7" in file.read():
+                cli_output.error(
+                    f"The Terraform configuration generated by symflow CLI v{get_current_version()} is incompatible "
+                    f"with the configuration generated by symflow CLI v7.\n"
+                )
+                cli_output.actionable(
+                    f"Please use 'symflow migrate' to migrate your configuration. Or, for instructions on how to "
+                    f"migrate your configuration manually, visit the docs at "
+                    "https://docs.symops.com/docs/migrating-generated-files-from-symflow-v7-to-v8"
+                    "\n"
+                )
+                # We found a file generated by a previous major version. Confirm if the user wishes to proceed anyway.
+                # If the user responds with yes, then this method returns None and the generate command will proceed.
+                # If the user responds with no (default), then this method will abort the generate command.
+                cli_output.error_confirm("Proceed anyway?", abort=True, default=False)
+
+
 def get_valid_flow_name(candidate: str, generator_cls: Type[FlowGeneration]) -> Optional[str]:
     """Interactively validate that a given string:
 
     - Could be used as a Flow slug
     - Could be used as a sym_flow Terraform resource name
     - Will not conflict with an existing Flow name
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/init.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/login.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/organization/organization_configure_mfa.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/organization/organization_configure_mfa.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/resources/list.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/resources/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/resources/resources.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/resources/resources.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/services/click/external_id_option.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/services/click/external_id_option.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/services/click/inquirer_choice.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/services/click/inquirer_choice.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/services/click/service_type_choice.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/services/click/service_type_choice.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/services/click/service_type_option.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/services/click/service_type_option.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/services/hooks/slack_delete.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/services/hooks/slack_delete.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/services/services.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/services/services.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/services/services_delete.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/services/services_delete.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/services/services_list.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/services/services_list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/services/services_update.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/services/services_update.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/status.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/symflow.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/symflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from sym.flow.cli.commands.bots import bots_commands
 from sym.flow.cli.commands.config import config_commands
 from sym.flow.cli.commands.docs import docs
 from sym.flow.cli.commands.domains import domains_commands
 from sym.flow.cli.commands.generate import generate
 from sym.flow.cli.commands.init import init
 from sym.flow.cli.commands.login import login, logout
+from sym.flow.cli.commands.migrate import migrate
 from sym.flow.cli.commands.organization import organization_commands
 from sym.flow.cli.commands.resources import resources_commands
 from sym.flow.cli.commands.services import services_commands
 from sym.flow.cli.commands.status import status
 from sym.flow.cli.commands.tokens import tokens_commands
 from sym.flow.cli.commands.users import users_commands
 from sym.flow.cli.commands.version import version
@@ -48,15 +49,15 @@
     """
 
     options.debug = debug
     if sym_jwt := os.getenv("SYM_JWT"):
         options.set_access_token(sym_jwt)
     options.set_api_url(api_url)
     options.set_auth_url(auth_url)
-    options.dprint(auth_url=auth_url, api_url=api_url)
+    options.dprint(f"SYM_AUTH_URL={auth_url}, SYM_API_URL={api_url}")
 
     maybe_display_update_message()
 
 
 symflow.add_command(version)
 symflow.add_command(login)
 symflow.add_command(logout)
@@ -68,7 +69,8 @@
 symflow.add_command(users_commands)
 symflow.add_command(config_commands)
 symflow.add_command(tokens_commands)
 symflow.add_command(bots_commands)
 symflow.add_command(resources_commands)
 symflow.add_command(domains_commands)
 symflow.add_command(docs)
+symflow.add_command(migrate)
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/tokens/issue.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/tokens/issue.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/tokens/list.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/tokens/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/tokens/revoke.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/tokens/revoke.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/tokens/tokens.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/tokens/tokens.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/create.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/create.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/delete.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/delete.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/delete_identity.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/delete_identity.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/list.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/list.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/list_identities.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/list_identities.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/set_role.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/set_role.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/update.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/update.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/update_identity.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/update_identity.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/update_name.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/update_name.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/users.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/users.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/commands/users/utils.py` & `sym_flow_cli-8.0.0/sym/flow/cli/commands/users/utils.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/errors.py` & `sym_flow_cli-8.0.0/sym/flow/cli/errors.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/api.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/api.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/api_operations.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/api_operations.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/approval_only.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/approval_only.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/aws_iam.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/aws_iam.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     flows,
 )
 
 from .aws import AWSFlowGeneration
 
 
 class AWSIAMFlowGeneration(AWSFlowGeneration):
-    REQUIRES_AWS: bool = True
-
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         self.role_name: str = ""
 
         while not self.role_name:
             role_name = click.prompt(
@@ -53,15 +51,15 @@
     def is_valid_aws_role_name(self, string):
         # Matches PascalCase, plus underscores b/c of AWS role naming
         return bool(re.match(r"([A-Z]+[a-z0-9_]+)+", string))
 
     def generate(self) -> None:
         """Generate the impl and Terraform files required to configure an AWS IAM Flow."""
         # Generate any core requirements that don't already exist in this directory.
-        self._generate_runtime_tf()
+        self._append_connector_module("runtime_connector")
         self._create_impls_directory()
         self._add_runtime_id_to_environment()
         self._append_connector_module("iam_connector")
 
         # Generate the AWS IAM specific files.
         self._generate_impl()
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/aws_lambda.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/aws_lambda.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     flows,
 )
 
 from .aws import AWSFlowGeneration
 
 
 class AWSLambdaFlowGeneration(AWSFlowGeneration):
-    REQUIRES_AWS: bool = True
-
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         self.aws_region: Optional[str] = self._get_aws_region()
 
     @property
     def impl_filepath(self) -> str:
@@ -36,15 +34,15 @@
         if Path(self.lambda_src_directory).exists():
             cli_output.fail(
                 f"The directory or file {self.lambda_src_directory} already exists.",
                 hint=f"Please try again with a unique Flow name.",
             )
 
         # Generate any core requirements that don't already exist in this directory.
-        self._generate_runtime_tf()
+        self._append_connector_module("runtime_connector")
         self._create_impls_directory()
         self._add_runtime_id_to_environment()
 
         # Generate the AWS Lambda specific files.
         self._generate_impl(source_file="lambda_impl.txt")
 
         with open(self.flow_tf_filepath, "w") as f:
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/aws_sso.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/aws_sso.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,21 @@
 from typing import Optional
 
 import click
 import hcl2
 import inquirer
 
 import sym.flow.cli.helpers.output as cli_output
-from sym.flow.cli.code_generation_templates import (  # import the *package* containing the impl.txt file
-    core,
-    flows,
-)
-from sym.flow.cli.helpers.terraform import get_terraform_resource
+from sym.flow.cli.code_generation_templates import flows
+from sym.flow.cli.helpers.terraform import get_terraform_module
 
 from .aws import AWSFlowGeneration
 
 
 class AWSSSOFlowGeneration(AWSFlowGeneration):
-    REQUIRES_AWS: bool = True
-
     SYM_SSO_PROFILE = "sym-sso-provisioning"
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         # Ensure that they have an SSO Profile that will work with the generated aws_sso_connector.tf
         if not self.has_sym_sso_provisioning_profile():
@@ -96,21 +91,21 @@
     @classmethod
     def get_flow_tf_filepath(cls, flow_name: str, working_directory: str = ".") -> str:
         return f"{working_directory}/aws_sso_{cls._get_flow_resource_name(flow_name)}.tf"
 
     def generate(self) -> None:
         """Generate the impl and Terraform files required to configure an AWS SSO Flow."""
         # Generate any core requirements that don't already exist in this directory.
-        self._generate_runtime_tf()
+        self._append_connector_module("runtime_connector")
         self._create_impls_directory()
         self._add_runtime_id_to_environment()
 
         # Generate the AWS SSO specific files.
         self._append_connector_module("sso_connector")
-        self._append_runtime_sso_assume_roles()
+        self._add_sso_account_id_safelist()
 
         self._generate_impl()
 
         with open(self.flow_tf_filepath, "w") as f:
             aws_sso_targets = []
             aws_sso_target_ids = []
 
@@ -141,25 +136,56 @@
                 {
                     "SYM_TEMPLATE_VAR_AWS_SSO_TARGETS": "\n".join(aws_sso_targets),
                     "SYM_TEMPLATE_VAR_AWS_SSO_SYM_TARGET_IDS": ", ".join(aws_sso_target_ids),
                 },
             )
             f.write(aws_sso_tf)
 
-    def _append_runtime_sso_assume_roles(self) -> None:
-        """Parses the runtime.tf file and adds a policy to allow the Runtime Connector to assume roles in the SSO
-        account if it does not already exist."""
-
-        # Open the file in Read + Append mode
-        with open(self.runtime_tf_filepath, "a+") as f:
-            # Ensure that we read from the beginning of the file. "a+" can have different behavior
-            # depending on the OS.
-            f.seek(0)
-            # Parse the existing runtime.tf file into a dict
-            runtime_tf = hcl2.load(f)
-
-            # Check to see if an aws_iam_policy.assume_roles_sso resource is already defined, and append one if not.
-            if not get_terraform_resource(runtime_tf, "aws_iam_policy", "sso_assume_roles"):
-                # Append the assume_roles_sso resource
-                sso_assume_roles = pkg_resources.read_text(core, "runtime_sso_assume_roles.tf")
-                f.write("\n")
-                f.write(sso_assume_roles)
+    def _add_sso_account_id_safelist(self) -> None:
+        """Parses the connectors.tf file and adds the account ID safelist input to the runtime_connector module
+        if it does not yet exist
+        """
+
+        # Open the file in Read + Write mode
+        with open(self.connectors_tf_filepath, "r+") as f:
+            # Parse the existing connectors.tf into a dict, including line numbers
+            connectors_tf = hcl2.load(f, with_meta=True)
+
+            # The runtime_connector module is guaranteed to exist, because we append it at the beginning of the
+            # generation if it does not yet exist.
+            runtime_connector = get_terraform_module(connectors_tf, "runtime_connector")
+
+            # If the runtime_connector does not have the account_id_safelist input already defined, then we
+            # will want to replace the module with one that defines the SSO Account in the account_id_safelist
+            # and re-write the file.
+            if not runtime_connector.get("account_id_safelist"):
+                # Read the file as an array of lines
+                f.seek(0)
+                connector_tf_lines = f.readlines()
+
+                # The array index of the closing bracket of the runtime_connector module.
+                runtime_connector_end = runtime_connector["__end_line__"] - 1
+
+                # We want to insert the `account_id_safelist` right before the closing bracket of the module.
+                # Slice the file to get the contents before and after the closing bracket
+                before_closing_bracket = connector_tf_lines[0:runtime_connector_end]
+                closing_bracket_and_after = connector_tf_lines[runtime_connector_end:]
+                account_id_safelist_lines = [
+                    "  # Allow the Runtime Connector Role to assume IAM Roles in the SSO Account as well.\n",
+                    "  account_id_safelist = [data.aws_caller_identity.sso.account_id]\n",
+                ]
+
+                # Insert the account_id_safelist lines before the end of the runtime_connector module closing bracket
+                # and reconstruct the connectors.tf file.
+                updated_connectors_tf = before_closing_bracket + account_id_safelist_lines + closing_bracket_and_after
+
+                # Ensure the file pointer is pointing to the beginning of the file
+                f.seek(0)
+
+                # Write the updated contents to connectors.tf
+                for line in updated_connectors_tf:
+                    f.write(line)
+
+                # Truncate any trailing text after our file pointer to ensure that the file contains only the
+                # contents that we just wrote.
+                # See: https://stackoverflow.com/questions/6648493/how-to-open-a-file-for-both-reading-and-writing#comment100583908_15976014
+                f.truncate()
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/core.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 import re
 from abc import ABC, abstractmethod
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 import click
+import hcl2
 
 import sym.flow.cli.helpers.output as cli_output
 from sym.flow.cli.code_generation_templates import (  # import the *package* containing the tf files
     core,
     flows,
 )
+from sym.flow.cli.code_generation_templates.core import connectors
 from sym.flow.cli.errors import CliError
+from sym.flow.cli.helpers.terraform import get_terraform_module
 from sym.flow.cli.helpers.version import get_current_version
 
 # Slugs are only allowed to have letters, numbers, and dashes. This regex matches
 # all character that are NOT those.
 slug_disallowed_pattern = re.compile(r"[^a-zA-Z\d-]+")
 
 
@@ -37,15 +40,15 @@
 
     def __init__(self, flow_name: str, directory: str = ".") -> None:
         self.flow_name = flow_name
         self.generation_time = datetime.utcnow()
         self.symflow_version = str(get_current_version())
         self.working_directory = directory
 
-        # Subclasses will choose whether they need runtime.tf or not, so we may
+        # Subclasses will choose whether they need runtime_connector or not, so we may
         # not need aws_region. Set to None here so it's never undefined.
         self.aws_region: Optional[str] = None
 
     @property
     def flow_resource_name(self) -> str:
         """The name of the Flow used as a slug may have dashes, but used as a
         file name or Terraform resource should have underscores.
@@ -53,15 +56,19 @@
         return self._get_flow_resource_name(self.flow_name)
 
     @property
     def secrets_tf_filepath(self):
         return f"{self.working_directory}/secrets.tf"
 
     @property
-    def runtime_tf_filepath(self):
+    def connectors_tf_filepath(self) -> str:
+        return f"{self.working_directory}/connectors.tf"
+
+    @property
+    def deprecated_runtime_tf_filepath(self):
         return f"{self.working_directory}/runtime.tf"
 
     @property
     def environment_tf_filepath(self):
         return f"{self.working_directory}/environment.tf"
 
     @property
@@ -110,35 +117,54 @@
     def final_instructions(self) -> None:
         """Optionally output instructions after code generation is complete for
         for the user to follow now or after `terraform apply` (e.g. instructions
         on how to set the value for a new AWS Secretsmanager Secret).
         """
 
     def _get_aws_region(self) -> Optional[str]:
-        """If a runtime.tf file would need to be generated, prompt the user for
+        """If a connectors.tf file would need to be generated, prompt the user for
         the AWS region to use.
         """
 
-        if not Path(self.runtime_tf_filepath).is_file():
+        if not Path(self.connectors_tf_filepath).is_file():
             return click.prompt(
                 click.style("What AWS region are your resources in?", bold=True), type=str, default="us-east-1"
             )
 
-    def _generate_runtime_tf(self) -> None:
-        """Generate runtime.tf if it does not already exist."""
-
-        if not Path(self.runtime_tf_filepath).is_file():
+    def _append_connector_module(self, module_name: str):
+        """
+        Creates a `connectors.tf` if it does not yet exist, then appends the given connector module to the
+        end of the file if the module does not already exist.
+        Args:
+            module_name: The name of the module (e.g. "iam_connector"). Should match the template file name as well.
+        """
+        # Create connectors.tf if it does not yet exist.
+        if not Path(self.connectors_tf_filepath).is_file():
             if not self.aws_region:
-                raise MissingConfig(file_name="runtime.tf", name="aws_region")
-
-            runtime_tf = pkg_resources.read_text(core, "runtime.tf")
+                raise MissingConfig(file_name="connectors.tf", name="aws_region")
 
-            with open(self.runtime_tf_filepath, "w") as f:
-                runtime_tf = self._format_template(runtime_tf, {"SYM_TEMPLATE_VAR_AWS_REGION": self.aws_region})
-                f.write(runtime_tf)
+            base_connectors_tf = pkg_resources.read_text(connectors, "connectors.tf")
+            with open(self.connectors_tf_filepath, "w") as f:
+                base_connectors_tf = self._format_template(
+                    base_connectors_tf, {"SYM_TEMPLATE_VAR_AWS_REGION": self.aws_region}
+                )
+                f.write(base_connectors_tf)
+
+        # Open connectors.tf in Read + Append mode
+        with open(self.connectors_tf_filepath, "a+") as f:
+            # Ensure that we read from the beginning of the file. "a+" can have different behavior
+            # depending on the OS.
+            f.seek(0)
+            connectors_tf = hcl2.load(f)
+
+            # If the module does not already exist in connectors.tf, append it.
+            if not get_terraform_module(connectors_tf, module_name):
+                module_contents = pkg_resources.read_text(connectors, f"{module_name}.tf")
+                f.write("\n")
+                f.write(module_contents)
 
     def _generate_secrets_tf(self) -> None:
         """Generate secrets.tf if it does not already exist."""
 
         if not Path(self.secrets_tf_filepath).is_file():
             secrets_tf = pkg_resources.read_text(core, "secrets.tf")
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/code_generation/okta.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/code_generation/okta.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     @classmethod
     def get_flow_tf_filepath(cls, flow_name: str, working_directory: str = ".") -> str:
         return f"{working_directory}/okta_{cls._get_flow_resource_name(flow_name)}.tf"
 
     def generate(self) -> None:
         """Generate the impl and Terraform files required to configure an Okta Flow."""
         # Generate any core requirements that don't already exist in this directory.
-        self._generate_runtime_tf()
+        self._append_connector_module("runtime_connector")
         self._generate_secrets_tf()
         self._create_impls_directory()
 
         # Generate the Okta-specific files.
         self._generate_impl()
 
         with open(self.flow_tf_filepath, "w") as f:
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/config/config.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/config/config.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/config/lock.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/config/lock.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/config/thread_safe_file.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/config/thread_safe_file.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/global_options.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/global_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-import inspect
-import logging
 from dataclasses import dataclass
-from typing import Optional, Sequence
+from typing import Optional
 from urllib.parse import urlparse
 
+import sym.flow.cli.helpers.output as cli_output
 from sym.flow.cli.helpers.constants import DEFAULT_API_URL, DEFAULT_AUTH_URL
 
 
 @dataclass
 class GlobalOptions:
     api_url: str = DEFAULT_API_URL
     auth_url: str = DEFAULT_AUTH_URL
     access_token: Optional[str] = None
     debug: bool = False
 
-    def dprint(self, *s: Sequence[str], **kwargs):
+    def dprint(self, message: str):
         """Prints debug messages if `self.debug` is True"""
-
-        s = list(map(str, filter(None, s)))
-        if (s or kwargs) and self.debug:
-            message = " ".join(s)
-            if kwargs:
-                message += ": " + ",".join([f"{k}={v}" for k, v in kwargs.items()])
-            mod = inspect.getmodule(inspect.stack()[1][0])
-            logging.getLogger(mod.__name__ if mod else __name__).info(message)
+        if self.debug:
+            cli_output.info(message)
 
     @property
     def sym_api(self):
         from sym.flow.cli.helpers.api import SymAPI
 
         return SymAPI(self.api_url, self.access_token)
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/identity_operations.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/identity_operations.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/jwt.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/jwt.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/login/handler.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/login/handler.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/login/login_flow.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/login/login_flow.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/output.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/output.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/profile_operations.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/profile_operations.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/rest.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/rest.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/sentry.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/sentry.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/terraform.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/terraform.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     if not (resources := file_contents.get("resource")):
         return None
 
     # Resources of the same type are not grouped, they will be different items in the list
     # of resources. So look at each of them, make sure they're the right type, and then also
     # check their name. If both match, return it.
     for r in resources:
-        if r.get(type_) and r[type_].get(name):
+        if r.get(type_) and name in r[type_]:
             return r[type_][name]
 
     # We didn't find what we were looking for, so this lookup was a failure.
     return None
 
 
 def get_terraform_local_variable(file_contents: dict, name: str) -> Any:
@@ -83,7 +83,28 @@
     returns None.
     """
 
     if not (modules := file_contents.get("module")):
         return None
 
     return next((m[name] for m in modules if m.get(name)), None)
+
+
+def get_terraform_data_resource(file_contents: dict, type_: str, name: str) -> Optional[dict]:
+    """Get the value of a data resource from the given Terraform file, represented as
+    a dictionary parsed by hcl2. If the particular module name cannot be found,
+    returns None.
+    """
+
+    if not (data_resources := file_contents.get("data")):
+        return None
+
+    # Resources of the same type are not grouped, they will be different items in the list
+    # of resources. So look at each of them, make sure they're the right type, and then also
+    # check their name. If both match, return it.
+    for r in data_resources:
+        # Data resources might be empty objects, in which case we want to return the empty dict, not None
+        if r.get(type_) and name in r[type_]:
+            return r[type_][name]
+
+    # We didn't find what we were looking for, so this lookup was a failure.
+    return None
```

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/tracked_command.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/tracked_command.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/users.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/users.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/utils.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/helpers/version.py` & `sym_flow_cli-8.0.0/sym/flow/cli/helpers/version.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/models/resource.py` & `sym_flow_cli-8.0.0/sym/flow/cli/models/resource.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/models/service_type.py` & `sym_flow_cli-8.0.0/sym/flow/cli/models/service_type.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/models/token.py` & `sym_flow_cli-8.0.0/sym/flow/cli/models/token.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/sym/flow/cli/models/user.py` & `sym_flow_cli-8.0.0/sym/flow/cli/models/user.py`

 * *Files identical despite different names*

### Comparing `sym_flow_cli-7.4.0/setup.py` & `sym_flow_cli-8.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 ['sym',
  'sym.flow',
  'sym.flow.cli',
  'sym.flow.cli.code_generation_templates',
  'sym.flow.cli.code_generation_templates.core',
  'sym.flow.cli.code_generation_templates.core.connectors',
  'sym.flow.cli.code_generation_templates.flows',
+ 'sym.flow.cli.code_generation_templates.migration',
+ 'sym.flow.cli.code_generation_templates.migration.v8',
  'sym.flow.cli.commands',
  'sym.flow.cli.commands.bots',
  'sym.flow.cli.commands.config',
  'sym.flow.cli.commands.domains',
  'sym.flow.cli.commands.organization',
  'sym.flow.cli.commands.resources',
  'sym.flow.cli.commands.services',
  'sym.flow.cli.commands.services.click',
  'sym.flow.cli.commands.services.hooks',
  'sym.flow.cli.commands.tokens',
  'sym.flow.cli.commands.users',
  'sym.flow.cli.helpers',
  'sym.flow.cli.helpers.code_generation',
+ 'sym.flow.cli.helpers.code_generation.migration',
  'sym.flow.cli.helpers.config',
  'sym.flow.cli.helpers.login',
  'sym.flow.cli.models']
 
 package_data = \
 {'': ['*']}
 
@@ -47,15 +50,15 @@
  'tabulate>=0.8.7,<0.9.0']
 
 entry_points = \
 {'console_scripts': ['symflow = sym.flow.cli.symflow:symflow']}
 
 setup_kwargs = {
     'name': 'sym-flow-cli',
-    'version': '7.4.0',
+    'version': '8.0.0',
     'description': "Sym's Official CLI for Implementers",
     'long_description': '# sym-flow-cli\n\nThis is the official CLI for [Sym](https://symops.com/) Implementers. Check out the docs [here](https://docs.symops.com/docs/install-sym-flow).\n',
     'author': 'SymOps, Inc.',
     'author_email': 'pypi@symops.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://symops.com/',
```

### Comparing `sym_flow_cli-7.4.0/PKG-INFO` & `sym_flow_cli-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sym-flow-cli
-Version: 7.4.0
+Version: 8.0.0
 Summary: Sym's Official CLI for Implementers
 Home-page: https://symops.com/
 Author: SymOps, Inc.
 Author-email: pypi@symops.io
 Requires-Python: >=3.8,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


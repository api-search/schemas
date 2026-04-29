---
description: API_Entities_PlanLimit model
layout: schema
name: API_Entities_PlanLimit
properties_list:
- description: ''
  name: ci_pipeline_size
  type: integer
- description: ''
  name: ci_active_jobs
  type: integer
- description: ''
  name: ci_project_subscriptions
  type: integer
- description: ''
  name: ci_pipeline_schedules
  type: integer
- description: ''
  name: ci_needs_size_limit
  type: integer
- description: ''
  name: ci_registered_group_runners
  type: integer
- description: ''
  name: ci_registered_project_runners
  type: integer
- description: ''
  name: conan_max_file_size
  type: integer
- description: ''
  name: enforcement_limit
  type: integer
- description: ''
  name: generic_packages_max_file_size
  type: integer
- description: ''
  name: helm_max_file_size
  type: integer
- description: ''
  name: limits_history
  type: object
- description: ''
  name: maven_max_file_size
  type: integer
- description: ''
  name: notification_limit
  type: integer
- description: ''
  name: npm_max_file_size
  type: integer
- description: ''
  name: nuget_max_file_size
  type: integer
- description: ''
  name: pipeline_hierarchy_size
  type: integer
- description: ''
  name: pypi_max_file_size
  type: integer
- description: ''
  name: terraform_module_max_file_size
  type: integer
- description: ''
  name: storage_size_limit
  type: integer
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-application-api_entities_plan-limit-schema.json
slug: gitlab-api-v4-application-api_entities_plan-limit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-application-api_entities_plan-limit-schema.json\",\n  \"title\": \"API_Entities_PlanLimit\",\n  \"description\": \"API_Entities_PlanLimit model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ci_pipeline_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 0\n    },\n    \"ci_active_jobs\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 0\n    },\n    \"ci_project_subscriptions\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 2\n    },\n    \"ci_pipeline_schedules\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 10\n    },\n    \"ci_needs_size_limit\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 50\n    },\n  \
  \  \"ci_registered_group_runners\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1000\n    },\n    \"ci_registered_project_runners\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1000\n    },\n    \"conan_max_file_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 3221225472\n    },\n    \"enforcement_limit\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 15000\n    },\n    \"generic_packages_max_file_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 5368709120\n    },\n    \"helm_max_file_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 5242880\n    },\n    \"limits_history\": {\n      \"type\": \"object\",\n      \"properties\": {},\n      \"example\": \"{\\\"enforcement_limit\\\"=>[{\\\"timestamp\\\"=>1686909124, \\\"user_id\\\"=>1, \\\"username\\\"=>\\\"x\\\
  \", \\\"value\\\"=>5}],\\n                   \\\"notification_limit\\\"=>[{\\\"timestamp\\\"=>1686909124, \\\"user_id\\\"=>2, \\\"username\\\"=>\\\"y\\\", \\\"value\\\"=>7}]}\"\n    },\n    \"maven_max_file_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 3221225472\n    },\n    \"notification_limit\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 15000\n    },\n    \"npm_max_file_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 524288000\n    },\n    \"nuget_max_file_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 524288000\n    },\n    \"pipeline_hierarchy_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1000\n    },\n    \"pypi_max_file_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 3221225472\n    },\n    \"terraform_module_max_file_size\": {\n\
  \      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1073741824\n    },\n    \"storage_size_limit\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 15000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-application-api_entities_plan-limit-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_PlanLimit
---

---
description: ''
layout: schema
name: RollbackConfiguration
properties_list:
- description: The triggers to monitor during stack creation or update.
  name: RollbackTriggers
  type: array
- description: The amount of time to monitor after stack deployment.
  name: MonitoringTimeInMinutes
  type: integer
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-rollback-configuration-schema.json
slug: cloudformation-rollback-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RollbackConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RollbackTriggers\": {\n      \"type\": \"array\",\n      \"description\": \"The triggers to monitor during stack creation or update.\"\n    },\n    \"MonitoringTimeInMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time to monitor after stack deployment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-rollback-configuration-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: RollbackConfiguration
---

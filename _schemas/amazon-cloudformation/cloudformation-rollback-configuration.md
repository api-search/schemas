---
description: RollbackConfiguration schema
layout: schema
name: RollbackConfiguration
properties_list:
- description: ''
  name: RollbackTriggers
  type: array
- description: ''
  name: MonitoringTimeInMinutes
  type: integer
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-rollback-configuration-schema.json
slug: cloudformation-rollback-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-rollback-configuration-schema.json\",\n  \"title\": \"RollbackConfiguration\",\n  \"description\": \"RollbackConfiguration schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RollbackTriggers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Arn\": {\n            \"type\": \"string\"\n          },\n          \"Type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"MonitoringTimeInMinutes\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-rollback-configuration-schema.json
tags:
- AWS
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: RollbackConfiguration
---

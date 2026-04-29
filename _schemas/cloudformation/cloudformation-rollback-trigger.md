---
description: ''
layout: schema
name: RollbackTrigger
properties_list:
- description: The Amazon Resource Name (ARN) of the rollback trigger.
  name: Arn
  type: string
- description: The resource type of the rollback trigger.
  name: Type
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-rollback-trigger-schema.json
slug: cloudformation-rollback-trigger
source_filename: cloudformation-rollback-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RollbackTrigger\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the rollback trigger.\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type of the rollback trigger.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-rollback-trigger-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: RollbackTrigger
---

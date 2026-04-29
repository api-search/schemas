---
description: ''
layout: schema
name: StackSetOperationPreferences
properties_list:
- description: ''
  name: RegionConcurrencyType
  type: string
- description: ''
  name: RegionOrder
  type: array
- description: ''
  name: FailureToleranceCount
  type: integer
- description: ''
  name: FailureTolerancePercentage
  type: integer
- description: ''
  name: MaxConcurrentCount
  type: integer
- description: ''
  name: MaxConcurrentPercentage
  type: integer
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-set-operation-preferences-schema.json
slug: cloudformation-stack-set-operation-preferences
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackSetOperationPreferences\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RegionConcurrencyType\": {\n      \"type\": \"string\"\n    },\n    \"RegionOrder\": {\n      \"type\": \"array\"\n    },\n    \"FailureToleranceCount\": {\n      \"type\": \"integer\"\n    },\n    \"FailureTolerancePercentage\": {\n      \"type\": \"integer\"\n    },\n    \"MaxConcurrentCount\": {\n      \"type\": \"integer\"\n    },\n    \"MaxConcurrentPercentage\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-set-operation-preferences-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackSetOperationPreferences
---

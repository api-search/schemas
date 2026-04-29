---
description: ''
layout: schema
name: StackSetSummary
properties_list:
- description: ''
  name: StackSetName
  type: string
- description: ''
  name: StackSetId
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: PermissionModel
  type: string
- description: ''
  name: DriftStatus
  type: string
- description: ''
  name: LastDriftCheckTimestamp
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-set-summary-schema.json
slug: cloudformation-stack-set-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackSetSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackSetName\": {\n      \"type\": \"string\"\n    },\n    \"StackSetId\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    },\n    \"PermissionModel\": {\n      \"type\": \"string\"\n    },\n    \"DriftStatus\": {\n      \"type\": \"string\"\n    },\n    \"LastDriftCheckTimestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-set-summary-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackSetSummary
---

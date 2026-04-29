---
description: ''
layout: schema
name: StackSet
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
  name: TemplateBody
  type: string
- description: ''
  name: Parameters
  type: array
- description: ''
  name: Capabilities
  type: array
- description: ''
  name: Tags
  type: array
- description: ''
  name: StackSetARN
  type: string
- description: ''
  name: AdministrationRoleARN
  type: string
- description: ''
  name: ExecutionRoleName
  type: string
- description: ''
  name: PermissionModel
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-set-schema.json
slug: cloudformation-stack-set
source_filename: cloudformation-stack-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackSet\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackSetName\": {\n      \"type\": \"string\"\n    },\n    \"StackSetId\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\"\n    },\n    \"TemplateBody\": {\n      \"type\": \"string\"\n    },\n    \"Parameters\": {\n      \"type\": \"array\"\n    },\n    \"Capabilities\": {\n      \"type\": \"array\"\n    },\n    \"Tags\": {\n      \"type\": \"array\"\n    },\n    \"StackSetARN\": {\n      \"type\": \"string\"\n    },\n    \"AdministrationRoleARN\": {\n      \"type\": \"string\"\n    },\n    \"ExecutionRoleName\": {\n      \"type\": \"string\"\n    },\n    \"PermissionModel\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-set-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackSet
---

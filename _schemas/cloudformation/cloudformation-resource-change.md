---
description: ''
layout: schema
name: ResourceChange
properties_list:
- description: ''
  name: Action
  type: string
- description: ''
  name: LogicalResourceId
  type: string
- description: ''
  name: PhysicalResourceId
  type: string
- description: ''
  name: ResourceType
  type: string
- description: ''
  name: Replacement
  type: string
- description: ''
  name: Scope
  type: array
- description: ''
  name: Details
  type: array
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-resource-change-schema.json
slug: cloudformation-resource-change
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceChange\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"type\": \"string\"\n    },\n    \"LogicalResourceId\": {\n      \"type\": \"string\"\n    },\n    \"PhysicalResourceId\": {\n      \"type\": \"string\"\n    },\n    \"ResourceType\": {\n      \"type\": \"string\"\n    },\n    \"Replacement\": {\n      \"type\": \"string\"\n    },\n    \"Scope\": {\n      \"type\": \"array\"\n    },\n    \"Details\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-resource-change-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ResourceChange
---

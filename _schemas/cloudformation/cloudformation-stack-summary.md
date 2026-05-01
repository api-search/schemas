---
description: ''
layout: schema
name: StackSummary
properties_list:
- description: ''
  name: StackId
  type: string
- description: ''
  name: StackName
  type: string
- description: ''
  name: TemplateDescription
  type: string
- description: ''
  name: CreationTime
  type: string
- description: ''
  name: LastUpdatedTime
  type: string
- description: ''
  name: DeletionTime
  type: string
- description: ''
  name: StackStatusReason
  type: string
- description: ''
  name: ParentId
  type: string
- description: ''
  name: RootId
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-summary-schema.json
slug: cloudformation-stack-summary
source_filename: cloudformation-stack-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackId\": {\n      \"type\": \"string\"\n    },\n    \"StackName\": {\n      \"type\": \"string\"\n    },\n    \"TemplateDescription\": {\n      \"type\": \"string\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\"\n    },\n    \"LastUpdatedTime\": {\n      \"type\": \"string\"\n    },\n    \"DeletionTime\": {\n      \"type\": \"string\"\n    },\n    \"StackStatusReason\": {\n      \"type\": \"string\"\n    },\n    \"ParentId\": {\n      \"type\": \"string\"\n    },\n    \"RootId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-summary-schema.json
tags:
- Automation
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackSummary
---

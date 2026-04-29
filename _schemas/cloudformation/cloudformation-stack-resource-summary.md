---
description: ''
layout: schema
name: StackResourceSummary
properties_list:
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
  name: LastUpdatedTimestamp
  type: string
- description: ''
  name: ResourceStatus
  type: string
- description: ''
  name: ResourceStatusReason
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-stack-resource-summary-schema.json
slug: cloudformation-stack-resource-summary
source_filename: cloudformation-stack-resource-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackResourceSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogicalResourceId\": {\n      \"type\": \"string\"\n    },\n    \"PhysicalResourceId\": {\n      \"type\": \"string\"\n    },\n    \"ResourceType\": {\n      \"type\": \"string\"\n    },\n    \"LastUpdatedTimestamp\": {\n      \"type\": \"string\"\n    },\n    \"ResourceStatus\": {\n      \"type\": \"string\"\n    },\n    \"ResourceStatusReason\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-stack-resource-summary-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: StackResourceSummary
---

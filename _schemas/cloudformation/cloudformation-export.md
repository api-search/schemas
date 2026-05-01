---
description: ''
layout: schema
name: Export
properties_list:
- description: The stack that contains the exported output value.
  name: ExportingStackId
  type: string
- description: The name of the exported output value.
  name: Name
  type: string
- description: The value of the exported output.
  name: Value
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-export-schema.json
slug: cloudformation-export
source_filename: cloudformation-export-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Export\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ExportingStackId\": {\n      \"type\": \"string\",\n      \"description\": \"The stack that contains the exported output value.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the exported output value.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the exported output.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-export-schema.json
tags:
- Automation
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: Export
---

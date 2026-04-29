---
description: ''
layout: schema
name: Output
properties_list:
- description: The key associated with the output.
  name: OutputKey
  type: string
- description: The value associated with the output.
  name: OutputValue
  type: string
- description: User-defined description.
  name: Description
  type: string
- description: The name of the export associated with the output.
  name: ExportName
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-output-schema.json
slug: cloudformation-output
source_filename: cloudformation-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Output\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputKey\": {\n      \"type\": \"string\",\n      \"description\": \"The key associated with the output.\"\n    },\n    \"OutputValue\": {\n      \"type\": \"string\",\n      \"description\": \"The value associated with the output.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined description.\"\n    },\n    \"ExportName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the export associated with the output.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-output-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: Output
---

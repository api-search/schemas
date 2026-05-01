---
description: ''
layout: schema
name: Parameter
properties_list:
- description: The key associated with the parameter.
  name: ParameterKey
  type: string
- description: The input value associated with the parameter.
  name: ParameterValue
  type: string
- description: Use the existing parameter value during stack updates.
  name: UsePreviousValue
  type: boolean
- description: The value that resolves to for SSM parameter types.
  name: ResolvedValue
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-parameter-schema.json
slug: cloudformation-parameter
source_filename: cloudformation-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Parameter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterKey\": {\n      \"type\": \"string\",\n      \"description\": \"The key associated with the parameter.\"\n    },\n    \"ParameterValue\": {\n      \"type\": \"string\",\n      \"description\": \"The input value associated with the parameter.\"\n    },\n    \"UsePreviousValue\": {\n      \"type\": \"boolean\",\n      \"description\": \"Use the existing parameter value during stack updates.\"\n    },\n    \"ResolvedValue\": {\n      \"type\": \"string\",\n      \"description\": \"The value that resolves to for SSM parameter types.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-parameter-schema.json
tags:
- Automation
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: Parameter
---

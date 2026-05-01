---
description: Parameter schema
layout: schema
name: Parameter
properties_list:
- description: ''
  name: ParameterKey
  type: string
- description: ''
  name: ParameterValue
  type: string
- description: ''
  name: UsePreviousValue
  type: boolean
- description: ''
  name: ResolvedValue
  type: string
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-parameter-schema.json
slug: cloudformation-parameter
source_filename: cloudformation-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-parameter-schema.json\",\n  \"title\": \"Parameter\",\n  \"description\": \"Parameter schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterKey\": {\n      \"type\": \"string\"\n    },\n    \"ParameterValue\": {\n      \"type\": \"string\"\n    },\n    \"UsePreviousValue\": {\n      \"type\": \"boolean\"\n    },\n    \"ResolvedValue\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-parameter-schema.json
tags:
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: Parameter
---

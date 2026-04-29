---
description: ''
layout: schema
name: ParameterDeclaration
properties_list:
- description: ''
  name: ParameterKey
  type: string
- description: ''
  name: DefaultValue
  type: string
- description: ''
  name: ParameterType
  type: string
- description: ''
  name: NoEcho
  type: boolean
- description: ''
  name: Description
  type: string
- description: ''
  name: ParameterConstraints
  type: object
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-parameter-declaration-schema.json
slug: cloudformation-parameter-declaration
source_filename: cloudformation-parameter-declaration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParameterDeclaration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterKey\": {\n      \"type\": \"string\"\n    },\n    \"DefaultValue\": {\n      \"type\": \"string\"\n    },\n    \"ParameterType\": {\n      \"type\": \"string\"\n    },\n    \"NoEcho\": {\n      \"type\": \"boolean\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"ParameterConstraints\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-parameter-declaration-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ParameterDeclaration
---

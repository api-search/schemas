---
description: ''
layout: schema
name: ModuleInfo
properties_list:
- description: A concatenated list of the module type hierarchy. For modules within other modules the format is Module1::Module2.
  name: TypeHierarchy
  type: string
- description: A concatenated list of the logical IDs of the module.
  name: LogicalIdHierarchy
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-module-info-schema.json
slug: cloudformation-module-info
source_filename: cloudformation-module-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModuleInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TypeHierarchy\": {\n      \"type\": \"string\",\n      \"description\": \"A concatenated list of the module type hierarchy. For modules within other modules the format is Module1::Module2.\"\n    },\n    \"LogicalIdHierarchy\": {\n      \"type\": \"string\",\n      \"description\": \"A concatenated list of the logical IDs of the module.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-module-info-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ModuleInfo
---

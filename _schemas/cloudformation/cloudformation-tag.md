---
description: ''
layout: schema
name: Tag
properties_list:
- description: Tag key.
  name: Key
  type: string
- description: Tag value.
  name: Value
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-tag-schema.json
slug: cloudformation-tag
source_filename: cloudformation-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"Tag key.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"Tag value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-tag-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: Tag
---

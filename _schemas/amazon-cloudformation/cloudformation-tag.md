---
description: Tag schema
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: string
- description: ''
  name: Value
  type: string
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-tag-schema.json
slug: cloudformation-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Tag schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\"\n    },\n    \"Value\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-tag-schema.json
tags:
- AWS
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: Tag
---

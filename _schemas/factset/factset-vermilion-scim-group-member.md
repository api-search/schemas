---
description: ''
layout: schema
name: ScimGroupMember
properties_list:
- description: ''
  name: value
  type: string
- description: A callback link which can be used to get the information of the group
  name: $ref
  type: string
- description: ''
  name: type
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vermilion-scim-group-member-schema.json
slug: factset-vermilion-scim-group-member
source_filename: factset-vermilion-scim-group-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScimGroupMember\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"$ref\": {\n      \"type\": \"string\",\n      \"description\": \"A callback link which can be used to get the information of the group\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vermilion-scim-group-member-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ScimGroupMember
---

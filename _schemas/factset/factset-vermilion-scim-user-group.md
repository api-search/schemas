---
description: ''
layout: schema
name: ScimUserGroup
properties_list:
- description: ''
  name: value
  type: string
- description: A callback link which can be used to get the information of the user
  name: $ref
  type: string
- description: ''
  name: type
  type: string
- description: Name of the group
  name: display
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vermilion-scim-user-group-schema.json
slug: factset-vermilion-scim-user-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScimUserGroup\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"$ref\": {\n      \"type\": \"string\",\n      \"description\": \"A callback link which can be used to get the information of the user\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"display\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the group\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vermilion-scim-user-group-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ScimUserGroup
---

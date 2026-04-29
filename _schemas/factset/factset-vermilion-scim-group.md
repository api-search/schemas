---
description: ''
layout: schema
name: ScimGroup
properties_list:
- description: ''
  name: schemas
  type: array
- description: ''
  name: id
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: members
  type: array
- description: ''
  name: tenant
  type: string
- description: ''
  name: domainCode
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vermilion-scim-group-schema.json
slug: factset-vermilion-scim-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScimGroup\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"members\": {\n      \"type\": \"array\"\n    },\n    \"tenant\": {\n      \"type\": \"string\"\n    },\n    \"domainCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vermilion-scim-group-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ScimGroup
---

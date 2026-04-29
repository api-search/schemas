---
description: ''
layout: schema
name: ScimError
properties_list:
- description: ''
  name: schemas
  type: array
- description: ''
  name: detail
  type: string
- description: ''
  name: status
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vermilion-scim-error-schema.json
slug: factset-vermilion-scim-error
source_filename: factset-vermilion-scim-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScimError\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\"\n    },\n    \"detail\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vermilion-scim-error-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ScimError
---

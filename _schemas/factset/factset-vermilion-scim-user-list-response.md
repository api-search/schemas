---
description: ''
layout: schema
name: ScimUserListResponse
properties_list:
- description: ''
  name: totalResults
  type: integer
- description: ''
  name: itemsPerPage
  type: integer
- description: ''
  name: startIndex
  type: integer
- description: ''
  name: Resources
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vermilion-scim-user-list-response-schema.json
slug: factset-vermilion-scim-user-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScimUserListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalResults\": {\n      \"type\": \"integer\"\n    },\n    \"itemsPerPage\": {\n      \"type\": \"integer\"\n    },\n    \"startIndex\": {\n      \"type\": \"integer\"\n    },\n    \"Resources\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vermilion-scim-user-list-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ScimUserListResponse
---

---
description: ''
layout: schema
name: SMRetrieveResponse
properties_list:
- description: ''
  name: securityName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: asofdate
  type: string
- description: ''
  name: errors
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-security-modeling-sm-retrieve-response-schema.json
slug: factset-security-modeling-sm-retrieve-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SMRetrieveResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"asofdate\": {\n      \"type\": \"string\"\n    },\n    \"errors\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-security-modeling-sm-retrieve-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: SMRetrieveResponse
---

---
description: ''
layout: schema
name: DataRequest
properties_list:
- description: ''
  name: '@type'
  type: string
- description: ''
  name: identifier
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: universe
  type: string
- description: ''
  name: fieldList
  type: string
- description: ''
  name: trigger
  type: string
- description: ''
  name: formatting
  type: object
- description: ''
  name: status
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-data-license-data-request-schema.json
slug: bloomberg-data-license-data-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"universe\": {\n      \"type\": \"string\"\n    },\n    \"fieldList\": {\n      \"type\": \"string\"\n    },\n    \"trigger\": {\n      \"type\": \"string\"\n    },\n    \"formatting\": {\n      \"type\": \"object\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-data-license-data-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: DataRequest
---

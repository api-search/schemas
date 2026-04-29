---
description: ''
layout: schema
name: RequestCreate
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
- description: URI reference to the universe resource
  name: universe
  type: string
- description: URI reference to the field list resource
  name: fieldList
  type: string
- description: URI reference to the trigger resource
  name: trigger
  type: string
- description: ''
  name: formatting
  type: object
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-data-license-request-create-schema.json
slug: bloomberg-data-license-request-create
source_filename: bloomberg-data-license-request-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequestCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"universe\": {\n      \"type\": \"string\",\n      \"description\": \"URI reference to the universe resource\"\n    },\n    \"fieldList\": {\n      \"type\": \"string\",\n      \"description\": \"URI reference to the field list resource\"\n    },\n    \"trigger\": {\n      \"type\": \"string\",\n      \"description\": \"URI reference to the trigger resource\"\n    },\n    \"formatting\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-data-license-request-create-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: RequestCreate
---

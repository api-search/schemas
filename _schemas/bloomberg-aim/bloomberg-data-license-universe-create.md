---
description: ''
layout: schema
name: UniverseCreate
properties_list:
- description: ''
  name: '@type'
  type: string
- description: Unique universe identifier
  name: identifier
  type: string
- description: Human-readable universe title
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: contains
  type: array
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-data-license-universe-create-schema.json
slug: bloomberg-data-license-universe-create
source_filename: bloomberg-data-license-universe-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UniverseCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique universe identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable universe title\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"contains\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-data-license-universe-create-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: UniverseCreate
---

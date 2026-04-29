---
description: ''
layout: schema
name: InstrumentListRequest
properties_list:
- description: Search string for instrument lookup
  name: query
  type: string
- description: Maximum number of results to return
  name: maxResults
  type: integer
- description: Filter by Bloomberg yellow key
  name: yellowKeyFilter
  type: string
- description: Two-letter language code
  name: languageOverride
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-instrument-list-request-schema.json
slug: bloomberg-http-instrument-list-request
source_filename: bloomberg-http-instrument-list-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstrumentListRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Search string for instrument lookup\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results to return\"\n    },\n    \"yellowKeyFilter\": {\n      \"type\": \"string\",\n      \"description\": \"Filter by Bloomberg yellow key\"\n    },\n    \"languageOverride\": {\n      \"type\": \"string\",\n      \"description\": \"Two-letter language code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-instrument-list-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: InstrumentListRequest
---

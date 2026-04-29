---
description: ''
layout: schema
name: FieldSearchRequest
properties_list:
- description: Search keyword or pattern
  name: searchSpec
  type: string
- description: ''
  name: returnFieldDocumentation
  type: boolean
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-field-search-request-schema.json
slug: bloomberg-http-field-search-request
source_filename: bloomberg-http-field-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FieldSearchRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"searchSpec\": {\n      \"type\": \"string\",\n      \"description\": \"Search keyword or pattern\"\n    },\n    \"returnFieldDocumentation\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-field-search-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: FieldSearchRequest
---

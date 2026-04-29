---
description: ''
layout: schema
name: CurveListRequest
properties_list:
- description: Search string for curve lookup
  name: query
  type: string
- description: ''
  name: maxResults
  type: integer
- description: Two-letter country code filter
  name: countryCode
  type: string
- description: Three-letter currency code filter
  name: currencyCode
  type: string
- description: Curve type filter
  name: type
  type: string
- description: ''
  name: subtype
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-curve-list-request-schema.json
slug: bloomberg-http-curve-list-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CurveListRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Search string for curve lookup\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Two-letter country code filter\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Three-letter currency code filter\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Curve type filter\"\n    },\n    \"subtype\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-curve-list-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: CurveListRequest
---

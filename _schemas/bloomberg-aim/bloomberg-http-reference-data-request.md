---
description: ''
layout: schema
name: ReferenceDataRequest
properties_list:
- description: List of security identifiers
  name: securities
  type: array
- description: List of Bloomberg field mnemonics
  name: fields
  type: array
- description: ''
  name: overrides
  type: array
- description: ''
  name: returnFormattedValue
  type: boolean
- description: ''
  name: useUTCTime
  type: boolean
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-reference-data-request-schema.json
slug: bloomberg-http-reference-data-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReferenceDataRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securities\": {\n      \"type\": \"array\",\n      \"description\": \"List of security identifiers\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"List of Bloomberg field mnemonics\"\n    },\n    \"overrides\": {\n      \"type\": \"array\"\n    },\n    \"returnFormattedValue\": {\n      \"type\": \"boolean\"\n    },\n    \"useUTCTime\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-reference-data-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: ReferenceDataRequest
---

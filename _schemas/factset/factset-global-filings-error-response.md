---
description: Error Response Object
layout: schema
name: ErrorResponse
properties_list:
- description: Errors Array Object
  name: errors
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-filings-error-response-schema.json
slug: factset-global-filings-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Error Response Object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Errors Array Object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-filings-error-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ErrorResponse
---

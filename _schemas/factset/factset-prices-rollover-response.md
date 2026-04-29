---
description: ''
layout: schema
name: rolloverResponse
properties_list:
- description: Array of `Database Rollover` objects.
  name: data
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-prices-rollover-response-schema.json
slug: factset-prices-rollover-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"rolloverResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of `Database Rollover` objects.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-prices-rollover-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: rolloverResponse
---

---
description: specifies the error message fields in the response
layout: schema
name: status
properties_list:
- description: An array containing errors
  name: errors
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-status-schema.json
slug: factset-tick-history-status
source_filename: factset-tick-history-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"status\",\n  \"type\": \"object\",\n  \"description\": \"specifies the error message fields in the response\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"An array containing errors\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-status-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: status
---

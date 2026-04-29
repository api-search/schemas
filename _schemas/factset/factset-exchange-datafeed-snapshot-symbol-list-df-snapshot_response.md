---
description: sample response
layout: schema
name: DFSnapshot_Response
properties_list:
- description: error value
  name: Error
  type: array
- description: first symbol from `ids` or `chain`
  name: symbol1
  type: array
- description: host name
  name: Host
  type: string
- description: second symbol from `ids` or `chain` list
  name: symbol2
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-exchange-datafeed-snapshot-symbol-list-df-snapshot_response-schema.json
slug: factset-exchange-datafeed-snapshot-symbol-list-df-snapshot_response
source_filename: factset-exchange-datafeed-snapshot-symbol-list-df-snapshot_response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DFSnapshot_Response\",\n  \"type\": \"object\",\n  \"description\": \"sample response\",\n  \"properties\": {\n    \"Error\": {\n      \"type\": \"array\",\n      \"description\": \"error value\"\n    },\n    \"symbol1\": {\n      \"type\": \"array\",\n      \"description\": \"first symbol from `ids` or `chain`\"\n    },\n    \"Host\": {\n      \"type\": \"string\",\n      \"description\": \"host name\"\n    },\n    \"symbol2\": {\n      \"type\": \"string\",\n      \"description\": \"second symbol from `ids` or `chain` list\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-exchange-datafeed-snapshot-symbol-list-df-snapshot_response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: DFSnapshot_Response
---

---
description: response for tick history
layout: schema
name: tickhistory_response
properties_list:
- description: Request Identification String.
  name: Requested ID
  type: string
- description: Single Requested Symbol or Security.
  name: Requested Symbol
  type: string
- description: Array of requested fields
  name: Requested Fields
  type: array
- description: ''
  name: Request Key
  type: string
- description: ''
  name: Error Code
  type: string
- description: Brief description of error response. Blank if successful.
  name: Error Description
  type: string
- description: Requested Field Names
  name: Field Names
  type: string
- description: Requested Field ID numbers 'FID'. Found in Data Service Manual.
  name: Field IDs
  type: number
- description: Requested Symbol Key, where :D represented delayed data.
  name: Key
  type: string
- description: Array of field values. Each value is returned for requested interval query.
  name: Values
  type: number
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-intraday-tick-history-tickhistory_response-schema.json
slug: factset-intraday-tick-history-tickhistory_response
source_filename: factset-intraday-tick-history-tickhistory_response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"tickhistory_response\",\n  \"type\": \"object\",\n  \"description\": \"response for tick history\",\n  \"properties\": {\n    \"Requested ID\": {\n      \"type\": \"string\",\n      \"description\": \"Request Identification String.\"\n    },\n    \"Requested Symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Single Requested Symbol or Security.\"\n    },\n    \"Requested Fields\": {\n      \"type\": \"array\",\n      \"description\": \"Array of requested fields \"\n    },\n    \"Request Key\": {\n      \"type\": \"string\"\n    },\n    \"Error Code\": {\n      \"type\": \"string\"\n    },\n    \"Error Description\": {\n      \"type\": \"string\",\n      \"description\": \"Brief description of error response. Blank if successful.\"\n    },\n    \"Field Names\": {\n      \"type\": \"string\",\n      \"description\": \"Requested Field Names\"\n    },\n    \"Field IDs\": {\n    \
  \  \"type\": \"number\",\n      \"description\": \"Requested Field ID numbers 'FID'. Found in Data Service Manual.\"\n    },\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"Requested Symbol Key, where :D represented delayed data.\"\n    },\n    \"Values\": {\n      \"type\": \"number\",\n      \"description\": \"Array of field values. Each value is returned for requested interval query.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-intraday-tick-history-tickhistory_response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: tickhistory_response
---

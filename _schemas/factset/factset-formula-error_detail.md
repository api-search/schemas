---
description: '`Error Object` is the response returned for an unsuccessful request.'
layout: schema
name: error_detail
properties_list:
- description: Unique identifier for the request. Also known as the chain id.
  name: id
  type: string
- description: Textual error code
  name: code
  type: string
- description: A short, human-readable summary of the problem
  name: title
  type: string
- description: timestamp in YYYY-MM-DD HH:MM:SS.SSS
  name: timestamp
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-formula-error_detail-schema.json
slug: factset-formula-error_detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"error_detail\",\n  \"type\": \"object\",\n  \"description\": \"`Error Object` is the response returned for an unsuccessful request.\\n\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the request. Also known as the chain id.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Textual error code\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"A short, human-readable summary of the problem\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"timestamp in YYYY-MM-DD HH:MM:SS.SSS\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-formula-error_detail-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: error_detail
---

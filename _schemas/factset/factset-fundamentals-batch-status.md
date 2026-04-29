---
description: Status information for an asynchronous batch request.
layout: schema
name: BatchStatus
properties_list:
- description: The batch request identifier.
  name: id
  type: string
- description: Time when the batch request started (Eastern Time Zone).
  name: startTime
  type: string
- description: Time when the batch request ended. Null if still processing.
  name: endTime
  type: '[''string'', ''null'']'
- description: Current batch processing status.
  name: status
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-batch-status-schema.json
slug: factset-fundamentals-batch-status
source_filename: factset-fundamentals-batch-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status information for an asynchronous batch request.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The batch request identifier.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the batch request started (Eastern Time Zone).\"\n    },\n    \"endTime\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Time when the batch request ended. Null if still processing.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current batch processing status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-batch-status-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: BatchStatus
---

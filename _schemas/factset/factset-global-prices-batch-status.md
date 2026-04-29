---
description: ''
layout: schema
name: BatchStatus
properties_list:
- description: the id of batch request.
  name: id
  type: string
- description: Time when the batch request is started. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.
  name: startTime
  type: string
- description: Time when the batch request is ended. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.
  name: endTime
  type: string
- description: ''
  name: status
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-prices-batch-status-schema.json
slug: factset-global-prices-batch-status
source_filename: factset-global-prices-batch-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"the id of batch request.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the batch request is started. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the batch request is ended. This is in Eastern Time Zone. The date-time format is expressed as [YYYY-MM-DD]T[HH:MM:SSS], following ISO 8601.\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-prices-batch-status-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: BatchStatus
---

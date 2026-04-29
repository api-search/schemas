---
description: ''
layout: schema
name: eventAdaptiveDataItem
properties_list:
- description: The id that was requested, ticker, cusip, factset entity id etc.
  name: requestId
  type: string
- description: Signal Id for this event.
  name: signalId
  type: string
- description: A JSON object that's compliant with MS adaptive card schema.
  name: adaptiveCard
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-signals-event-adaptive-data-item-schema.json
slug: factset-signals-event-adaptive-data-item
source_filename: factset-signals-event-adaptive-data-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"eventAdaptiveDataItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The id that was requested, ticker, cusip, factset entity id etc.\"\n    },\n    \"signalId\": {\n      \"type\": \"string\",\n      \"description\": \"Signal Id for this event.\"\n    },\n    \"adaptiveCard\": {\n      \"type\": \"object\",\n      \"description\": \"A JSON object that's compliant with MS adaptive card schema.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-signals-event-adaptive-data-item-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: eventAdaptiveDataItem
---

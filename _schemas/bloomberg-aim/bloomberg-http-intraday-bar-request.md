---
description: ''
layout: schema
name: IntradayBarRequest
properties_list:
- description: Single security identifier
  name: security
  type: string
- description: ''
  name: eventType
  type: string
- description: ''
  name: startDateTime
  type: string
- description: ''
  name: endDateTime
  type: string
- description: Bar interval in minutes
  name: interval
  type: integer
- description: ''
  name: gapFillInitialBar
  type: boolean
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-intraday-bar-request-schema.json
slug: bloomberg-http-intraday-bar-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntradayBarRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"security\": {\n      \"type\": \"string\",\n      \"description\": \"Single security identifier\"\n    },\n    \"eventType\": {\n      \"type\": \"string\"\n    },\n    \"startDateTime\": {\n      \"type\": \"string\"\n    },\n    \"endDateTime\": {\n      \"type\": \"string\"\n    },\n    \"interval\": {\n      \"type\": \"integer\",\n      \"description\": \"Bar interval in minutes\"\n    },\n    \"gapFillInitialBar\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-intraday-bar-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: IntradayBarRequest
---

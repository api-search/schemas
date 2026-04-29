---
description: ''
layout: schema
name: IntradayTickRequest
properties_list:
- description: Single security identifier
  name: security
  type: string
- description: ''
  name: eventTypes
  type: array
- description: Start of the time range
  name: startDateTime
  type: string
- description: End of the time range
  name: endDateTime
  type: string
- description: ''
  name: includeConditionCodes
  type: boolean
- description: ''
  name: includeExchangeCodes
  type: boolean
- description: ''
  name: includeBrokerCodes
  type: boolean
- description: ''
  name: includeRPSCodes
  type: boolean
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-intraday-tick-request-schema.json
slug: bloomberg-http-intraday-tick-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntradayTickRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"security\": {\n      \"type\": \"string\",\n      \"description\": \"Single security identifier\"\n    },\n    \"eventTypes\": {\n      \"type\": \"array\"\n    },\n    \"startDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Start of the time range\"\n    },\n    \"endDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"End of the time range\"\n    },\n    \"includeConditionCodes\": {\n      \"type\": \"boolean\"\n    },\n    \"includeExchangeCodes\": {\n      \"type\": \"boolean\"\n    },\n    \"includeBrokerCodes\": {\n      \"type\": \"boolean\"\n    },\n    \"includeRPSCodes\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-intraday-tick-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: IntradayTickRequest
---

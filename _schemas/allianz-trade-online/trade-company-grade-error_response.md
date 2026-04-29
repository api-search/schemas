---
description: Standard error response
layout: schema
name: ErrorResponse
properties_list:
- description: Error code
  name: code
  type: string
- description: Human-readable error description
  name: message
  type: string
- description: Request identifier for support reference
  name: requestId
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-company-grade-error_response-schema.json
slug: trade-company-grade-error_response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-company-grade-error_response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Request identifier for support reference\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-company-grade-error_response-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: ErrorResponse
---

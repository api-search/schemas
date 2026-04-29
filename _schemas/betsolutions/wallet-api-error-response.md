---
description: Error response returned when a request fails.
layout: schema
name: ErrorResponse
properties_list:
- description: Always false for error responses.
  name: success
  type: boolean
- description: Numeric error code.
  name: errorCode
  type: integer
- description: Human-readable error description.
  name: errorMessage
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-error-response-schema.json
slug: wallet-api-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Error response returned when a request fails.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Always false for error responses.\",\n      \"example\": false\n    },\n    \"errorCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric error code.\",\n      \"example\": 400\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description.\",\n      \"example\": \"Invalid hash signature.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-error-response-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: ErrorResponse
---

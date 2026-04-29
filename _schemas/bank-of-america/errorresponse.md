---
description: API error response
layout: schema
name: ErrorResponse
properties_list:
- description: Machine-readable error code
  name: errorCode
  type: string
- description: Human-readable error message
  name: message
  type: string
- description: Additional error details
  name: details
  type: array
- description: Request identifier for support
  name: requestId
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/errorresponse-schema.json
slug: errorresponse
source_filename: errorresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/errorresponse-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"API error response\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional error details\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Request identifier for support\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/errorresponse-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: ErrorResponse
---

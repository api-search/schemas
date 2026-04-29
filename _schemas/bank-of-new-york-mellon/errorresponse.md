---
description: API error response
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: errorCode
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: requestId
  type: string
- description: ''
  name: details
  type: array
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/errorresponse-schema.json
slug: errorresponse
source_filename: errorresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/errorresponse-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"API error response\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"requestId\": {\n      \"type\": \"string\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/errorresponse-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: ErrorResponse
---

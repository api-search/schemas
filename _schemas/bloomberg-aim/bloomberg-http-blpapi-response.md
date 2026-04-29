---
description: ''
layout: schema
name: BlpapiResponse
properties_list:
- description: HTTP status code
  name: statusCode
  type: integer
- description: ''
  name: message
  type: string
- description: ''
  name: data
  type: array
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-blpapi-response-schema.json
slug: bloomberg-http-blpapi-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlpapiResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"data\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-blpapi-response-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: BlpapiResponse
---

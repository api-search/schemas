---
description: ''
layout: schema
name: BlpapiRequest
properties_list:
- description: BLPAPI service URI (e.g., //blp/refdata)
  name: serviceUri
  type: string
- description: Name of the BLPAPI operation
  name: operationName
  type: string
- description: The operation-specific request payload
  name: requestObject
  type: object
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-http-blpapi-request-schema.json
slug: bloomberg-http-blpapi-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlpapiRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceUri\": {\n      \"type\": \"string\",\n      \"description\": \"BLPAPI service URI (e.g., //blp/refdata)\"\n    },\n    \"operationName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the BLPAPI operation\"\n    },\n    \"requestObject\": {\n      \"type\": \"object\",\n      \"description\": \"The operation-specific request payload\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-http-blpapi-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: BlpapiRequest
---

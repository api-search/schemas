---
description: Standard error response object.
layout: schema
name: Error Response
properties_list:
- description: Error code identifier.
  name: error
  type: string
- description: Human-readable error message.
  name: message
  type: string
- description: HTTP status code.
  name: statusCode
  type: integer
provider_name: albertsons
provider_slug: albertsons
schema_file: json-schema/retail-media-api-error-response-schema.json
slug: retail-media-api-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-error-response-schema.json\",\n  \"title\": \"Error Response\",\n  \"description\": \"Standard error response object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error code identifier.\",\n      \"example\": \"UNAUTHORIZED\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\",\n      \"example\": \"Invalid or missing bearer token.\"\n    },\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\",\n      \"example\": 401\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-error-response-schema.json
tags:
- Grocery
- Retail
- Retail Media
- Advertising
- Campaigns
- Analytics
- Consumer Goods
- Food
- Pharmacy
title: Error Response
---

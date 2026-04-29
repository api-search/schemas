---
description: Error response returned when a request fails.
layout: schema
name: ErrorResponse
properties_list:
- description: HTTP status code.
  name: status
  type: integer
- description: Error type or code.
  name: error
  type: string
- description: Human-readable description of the error.
  name: message
  type: string
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/recommendations-api-error-response-schema.json
slug: recommendations-api-error-response
source_filename: recommendations-api-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/recommendations-api-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Error response returned when a request fails.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\",\n      \"example\": 400\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error type or code.\",\n      \"example\": \"Bad Request\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the error.\",\n      \"example\": \"Invalid query parameter provided.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/recommendations-api-error-response-schema.json
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: ErrorResponse
---

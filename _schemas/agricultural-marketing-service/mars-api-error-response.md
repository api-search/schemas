---
description: Standard error response from the MARS API.
layout: schema
name: Error Response
properties_list:
- description: Error type or code.
  name: error
  type: string
- description: Human-readable error message.
  name: message
  type: string
- description: HTTP status code.
  name: status
  type: integer
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
schema_file: json-schema/mars-api-error-response-schema.json
slug: mars-api-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-error-response-schema.json\",\n  \"title\": \"Error Response\",\n  \"description\": \"Standard error response from the MARS API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error type or code.\",\n      \"example\": \"invalid_parameter\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\",\n      \"example\": \"The requested resource was not found.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\",\n      \"example\": 404\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-error-response-schema.json
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
title: Error Response
---

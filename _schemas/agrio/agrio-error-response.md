---
description: Standard error response.
layout: schema
name: Error Response
properties_list:
- description: Error code or type.
  name: error
  type: string
- description: Human-readable error message.
  name: message
  type: string
- description: HTTP status code.
  name: status
  type: integer
provider_name: agrio
provider_slug: agrio
schema_file: json-schema/agrio-error-response-schema.json
slug: agrio-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-error-response-schema.json\",\n  \"title\": \"Error Response\",\n  \"description\": \"Standard error response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error code or type.\",\n      \"example\": \"unauthorized\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\",\n      \"example\": \"Invalid or missing API key.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\",\n      \"example\": 401\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-error-response-schema.json
tags:
- Agriculture
- Plant Disease
- Pest Detection
- AI
- Crop Advisory
title: Error Response
---

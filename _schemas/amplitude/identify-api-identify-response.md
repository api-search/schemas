---
description: IdentifyResponse schema from Amplitude Identify API
layout: schema
name: IdentifyResponse
properties_list:
- description: The HTTP status code of the response.
  name: code
  type: integer
- description: The time the server received the request in milliseconds since epoch.
  name: server_upload_time
  type: integer
- description: The number of identify operations successfully processed.
  name: events_ingested
  type: integer
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/identify-api-identify-response-schema.json
slug: identify-api-identify-response
source_filename: identify-api-identify-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/identify-api-identify-response-schema.json\",\n  \"title\": \"IdentifyResponse\",\n  \"description\": \"IdentifyResponse schema from Amplitude Identify API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code of the response.\",\n      \"example\": 200\n    },\n    \"server_upload_time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The time the server received the request in milliseconds since epoch.\"\n    },\n    \"events_ingested\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of identify operations successfully processed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/identify-api-identify-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: IdentifyResponse
---

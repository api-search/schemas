---
description: UploadResponse schema from Amplitude HTTP V2 API
layout: schema
name: UploadResponse
properties_list:
- description: The HTTP status code of the response.
  name: code
  type: integer
- description: The number of events successfully ingested.
  name: events_ingested
  type: integer
- description: The size of the request payload in bytes.
  name: payload_size_bytes
  type: integer
- description: The time the server received the upload in milliseconds since epoch.
  name: server_upload_time
  type: integer
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/http-v2-api-upload-response-schema.json
slug: http-v2-api-upload-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/http-v2-api-upload-response-schema.json\",\n  \"title\": \"UploadResponse\",\n  \"description\": \"UploadResponse schema from Amplitude HTTP V2 API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code of the response.\",\n      \"example\": 200\n    },\n    \"events_ingested\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of events successfully ingested.\"\n    },\n    \"payload_size_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the request payload in bytes.\"\n    },\n    \"server_upload_time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The time the server received the upload in milliseconds since epoch.\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/http-v2-api-upload-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UploadResponse
---

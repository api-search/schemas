---
description: AttributionResponse schema from Amplitude Attribution API
layout: schema
name: AttributionResponse
properties_list:
- description: The HTTP status code of the response.
  name: code
  type: integer
- description: The number of events successfully ingested.
  name: events_ingested
  type: integer
- description: The time the server received the upload in milliseconds since epoch.
  name: server_upload_time
  type: integer
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/attribution-api-attribution-response-schema.json
slug: attribution-api-attribution-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/attribution-api-attribution-response-schema.json\",\n  \"title\": \"AttributionResponse\",\n  \"description\": \"AttributionResponse schema from Amplitude Attribution API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code of the response.\",\n      \"example\": 200\n    },\n    \"events_ingested\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of events successfully ingested.\"\n    },\n    \"server_upload_time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The time the server received the upload in milliseconds since epoch.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/attribution-api-attribution-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: AttributionResponse
---

---
description: DsarStatusResponse schema from Amplitude Data Subject Access Request API
layout: schema
name: DsarStatusResponse
properties_list:
- description: The unique identifier for the DSAR request.
  name: request_id
  type: string
- description: The processing status of the request.
  name: status
  type: string
- description: The URL to download the requested data. Only present when status is complete.
  name: download_url
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dsar-api-dsar-status-response-schema.json
slug: dsar-api-dsar-status-response
source_filename: dsar-api-dsar-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-dsar-status-response-schema.json\",\n  \"title\": \"DsarStatusResponse\",\n  \"description\": \"DsarStatusResponse schema from Amplitude Data Subject Access Request API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the DSAR request.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The processing status of the request.\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"complete\",\n        \"failed\"\n      ]\n    },\n    \"download_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to download the requested data. Only present when status is complete.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-dsar-status-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: DsarStatusResponse
---

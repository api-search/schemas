---
description: DsarResponse schema from Amplitude Data Subject Access Request API
layout: schema
name: DsarResponse
properties_list:
- description: The unique identifier for the DSAR request.
  name: request_id
  type: string
- description: The status of the request.
  name: status
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dsar-api-dsar-response-schema.json
slug: dsar-api-dsar-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-dsar-response-schema.json\",\n  \"title\": \"DsarResponse\",\n  \"description\": \"DsarResponse schema from Amplitude Data Subject Access Request API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the DSAR request.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-dsar-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: DsarResponse
---

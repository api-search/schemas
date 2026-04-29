---
description: DeletionResponse schema from Amplitude Data Subject Access Request API
layout: schema
name: DeletionResponse
properties_list:
- description: The day the deletion job is scheduled for processing.
  name: day
  type: string
- description: The status of the deletion request.
  name: status
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dsar-api-deletion-response-schema.json
slug: dsar-api-deletion-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-deletion-response-schema.json\",\n  \"title\": \"DeletionResponse\",\n  \"description\": \"DeletionResponse schema from Amplitude Data Subject Access Request API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"day\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The day the deletion job is scheduled for processing.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the deletion request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-deletion-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: DeletionResponse
---

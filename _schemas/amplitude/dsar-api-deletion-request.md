---
description: DeletionRequest schema from Amplitude Data Subject Access Request API
layout: schema
name: DeletionRequest
properties_list:
- description: Array of Amplitude internal user IDs to delete data for. Maximum 100 per request.
  name: amplitude_ids
  type: array
- description: Array of user IDs to delete data for. Maximum 100 per request.
  name: user_ids
  type: array
- description: The email address of the person requesting the deletion for audit purposes.
  name: requester
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dsar-api-deletion-request-schema.json
slug: dsar-api-deletion-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-deletion-request-schema.json\",\n  \"title\": \"DeletionRequest\",\n  \"description\": \"DeletionRequest schema from Amplitude Data Subject Access Request API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amplitude_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Array of Amplitude internal user IDs to delete data for. Maximum 100 per request.\",\n      \"maxItems\": 100,\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    },\n    \"user_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Array of user IDs to delete data for. Maximum 100 per request.\",\n      \"maxItems\": 100,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"requester\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The email address of the person requesting the deletion for audit purposes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-deletion-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: DeletionRequest
---

---
description: DeletionListResponse schema from Amplitude Data Subject Access Request API
layout: schema
name: DeletionListResponse
properties_list:
- description: Array of deletion request records.
  name: deletions
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dsar-api-deletion-list-response-schema.json
slug: dsar-api-deletion-list-response
source_filename: dsar-api-deletion-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-deletion-list-response-schema.json\",\n  \"title\": \"DeletionListResponse\",\n  \"description\": \"DeletionListResponse schema from Amplitude Data Subject Access Request API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deletions\": {\n      \"type\": \"array\",\n      \"description\": \"Array of deletion request records.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"day\": {\n            \"type\": \"string\",\n            \"format\": \"date\",\n            \"description\": \"The day the deletion job was scheduled.\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"The processing status of the deletion.\",\n            \"enum\": [\n              \"staging\",\n              \"submitted\"\
  ,\n              \"done\"\n            ]\n          },\n          \"amplitude_ids\": {\n            \"type\": \"array\",\n            \"description\": \"Array of Amplitude IDs included in the deletion.\",\n            \"items\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            }\n          },\n          \"user_ids\": {\n            \"type\": \"array\",\n            \"description\": \"Array of user IDs included in the deletion.\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-deletion-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: DeletionListResponse
---

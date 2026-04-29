---
description: DsarRequest schema from Amplitude Data Subject Access Request API
layout: schema
name: DsarRequest
properties_list:
- description: Array of user IDs to retrieve data for.
  name: user_ids
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dsar-api-dsar-request-schema.json
slug: dsar-api-dsar-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-dsar-request-schema.json\",\n  \"title\": \"DsarRequest\",\n  \"description\": \"DsarRequest schema from Amplitude Data Subject Access Request API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Array of user IDs to retrieve data for.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"user_ids\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dsar-api-dsar-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: DsarRequest
---

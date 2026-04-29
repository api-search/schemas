---
description: UserUnmapRequest schema from Amplitude User Mapping API
layout: schema
name: UserUnmapRequest
properties_list:
- description: An array of user mapping objects to reverse.
  name: mapping
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/user-mapping-api-user-unmap-request-schema.json
slug: user-mapping-api-user-unmap-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-mapping-api-user-unmap-request-schema.json\",\n  \"title\": \"UserUnmapRequest\",\n  \"description\": \"UserUnmapRequest schema from Amplitude User Mapping API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mapping\": {\n      \"type\": \"array\",\n      \"description\": \"An array of user mapping objects to reverse.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"global_user_id\",\n          \"user_id\"\n        ],\n        \"properties\": {\n          \"global_user_id\": {\n            \"type\": \"string\",\n            \"description\": \"The primary user ID that other identities will be mapped to.\"\n          },\n          \"user_id\": {\n            \"type\": \"string\",\n            \"description\": \"The user ID to map to the global_user_id.\"\n\
  \          },\n          \"unmap\": {\n            \"type\": \"boolean\",\n            \"description\": \"When true, removes the mapping instead of creating it.\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"mapping\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-mapping-api-user-unmap-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserUnmapRequest
---

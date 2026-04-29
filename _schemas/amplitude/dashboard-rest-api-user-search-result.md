---
description: UserSearchResult schema from Amplitude Dashboard REST API
layout: schema
name: UserSearchResult
properties_list:
- description: Array of matching users with their identifiers.
  name: matches
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/dashboard-rest-api-user-search-result-schema.json
slug: dashboard-rest-api-user-search-result
source_filename: dashboard-rest-api-user-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-user-search-result-schema.json\",\n  \"title\": \"UserSearchResult\",\n  \"description\": \"UserSearchResult schema from Amplitude Dashboard REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matches\": {\n      \"type\": \"array\",\n      \"description\": \"Array of matching users with their identifiers.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"user_id\": {\n            \"type\": \"string\",\n            \"description\": \"The user's user_id.\"\n          },\n          \"amplitude_id\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The user's Amplitude internal ID.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/dashboard-rest-api-user-search-result-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserSearchResult
---

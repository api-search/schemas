---
description: VersionListResponse schema from Amplitude Experiment Management API
layout: schema
name: VersionListResponse
properties_list:
- description: Array of version records.
  name: versions
  type: array
- description: A cursor for fetching the next page.
  name: nextCursor
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-version-list-response-schema.json
slug: experiment-management-api-version-list-response
source_filename: experiment-management-api-version-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-version-list-response-schema.json\",\n  \"title\": \"VersionListResponse\",\n  \"description\": \"VersionListResponse schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"Array of version records.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The version record ID.\"\n          },\n          \"flagId\": {\n            \"type\": \"string\",\n            \"description\": \"The flag or experiment ID.\"\n          },\n          \"version\": {\n            \"type\": \"integer\",\n            \"description\": \"The version number.\"\n          },\n  \
  \        \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the version was created.\"\n          },\n          \"createdBy\": {\n            \"type\": \"string\",\n            \"description\": \"The user who created this version.\"\n          }\n        }\n      }\n    },\n    \"nextCursor\": {\n      \"type\": \"string\",\n      \"description\": \"A cursor for fetching the next page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-version-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: VersionListResponse
---

---
description: FlagListResponse schema from Amplitude Experiment Management API
layout: schema
name: FlagListResponse
properties_list:
- description: Array of feature flag objects.
  name: flags
  type: array
- description: A cursor for fetching the next page of results.
  name: nextCursor
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-flag-list-response-schema.json
slug: experiment-management-api-flag-list-response
source_filename: experiment-management-api-flag-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-flag-list-response-schema.json\",\n  \"title\": \"FlagListResponse\",\n  \"description\": \"FlagListResponse schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flags\": {\n      \"type\": \"array\",\n      \"description\": \"Array of feature flag objects.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the flag.\"\n          },\n          \"projectId\": {\n            \"type\": \"string\",\n            \"description\": \"The project ID the flag belongs to.\"\n          },\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"The unique key used to reference\
  \ the flag in code.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the flag.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of the flag's purpose.\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the flag is enabled.\"\n          },\n          \"evaluationMode\": {\n            \"type\": \"string\",\n            \"description\": \"The evaluation mode, either local or remote.\",\n            \"enum\": [\n              \"local\",\n              \"remote\"\n            ]\n          },\n          \"bucketingKey\": {\n            \"type\": \"string\",\n            \"description\": \"The property used for bucketing users into variants.\"\n          },\n          \"bucketingSalt\": {\n            \"type\": \"string\",\n            \"description\": \"The salt used for hashing\
  \ during bucketing.\"\n          },\n          \"variants\": {\n            \"type\": \"array\",\n            \"description\": \"Array of variant configurations.\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/VariantConfig\"\n            }\n          },\n          \"deployments\": {\n            \"type\": \"array\",\n            \"description\": \"Array of deployment IDs the flag is deployed to.\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"segments\": {\n            \"type\": \"array\",\n            \"description\": \"Array of targeting segment configurations.\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Segment\"\n            }\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"description\": \"The current state of the flag.\",\n            \"enum\": [\n              \"draft\",\n              \"active\",\n              \"archived\"\
  \n            ]\n          }\n        }\n      }\n    },\n    \"nextCursor\": {\n      \"type\": \"string\",\n      \"description\": \"A cursor for fetching the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-flag-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: FlagListResponse
---

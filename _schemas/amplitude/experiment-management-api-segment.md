---
description: Segment schema from Amplitude Experiment Management API
layout: schema
name: Segment
properties_list:
- description: The display name of the segment.
  name: name
  type: string
- description: Array of targeting conditions that define this segment.
  name: conditions
  type: array
- description: The variant key to assign when this segment matches.
  name: variant
  type: string
- description: The percentage of matching users to include (0-100).
  name: percentage
  type: integer
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-segment-schema.json
slug: experiment-management-api-segment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-segment-schema.json\",\n  \"title\": \"Segment\",\n  \"description\": \"Segment schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the segment.\"\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"description\": \"Array of targeting conditions that define this segment.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The condition type.\"\n          },\n          \"prop\": {\n            \"type\": \"string\",\n            \"description\": \"The property to evaluate.\"\n          },\n          \"op\": {\n      \
  \      \"type\": \"string\",\n            \"description\": \"The comparison operator.\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"description\": \"The values to compare against.\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"variant\": {\n      \"type\": \"string\",\n      \"description\": \"The variant key to assign when this segment matches.\"\n    },\n    \"percentage\": {\n      \"type\": \"integer\",\n      \"description\": \"The percentage of matching users to include (0-100).\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-segment-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: Segment
---

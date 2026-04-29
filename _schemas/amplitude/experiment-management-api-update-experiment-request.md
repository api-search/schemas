---
description: UpdateExperimentRequest schema from Amplitude Experiment Management API
layout: schema
name: UpdateExperimentRequest
properties_list:
- description: The updated display name.
  name: name
  type: string
- description: The updated description.
  name: description
  type: string
- description: Whether the experiment should be enabled.
  name: enabled
  type: boolean
- description: Updated variant configurations.
  name: variants
  type: array
- description: Updated targeting segments.
  name: segments
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-update-experiment-request-schema.json
slug: experiment-management-api-update-experiment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-update-experiment-request-schema.json\",\n  \"title\": \"UpdateExperimentRequest\",\n  \"description\": \"UpdateExperimentRequest schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The updated display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The updated description.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the experiment should be enabled.\"\n    },\n    \"variants\": {\n      \"type\": \"array\",\n      \"description\": \"Updated variant configurations.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n    \
  \        \"type\": \"string\",\n            \"description\": \"The unique key for the variant.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the variant.\"\n          },\n          \"payload\": {\n            \"description\": \"An optional JSON payload associated with the variant.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of what this variant does.\"\n          },\n          \"rolloutWeight\": {\n            \"type\": \"integer\",\n            \"description\": \"The rollout weight as a percentage (0-100) controlling traffic allocation to this variant.\",\n            \"minimum\": 0,\n            \"maximum\": 100\n          }\n        }\n      }\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"Updated targeting segments.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the segment.\"\n          },\n          \"conditions\": {\n            \"type\": \"array\",\n            \"description\": \"Array of targeting conditions that define this segment.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"description\": \"The condition type.\"\n                },\n                \"prop\": {\n                  \"type\": \"string\",\n                  \"description\": \"The property to evaluate.\"\n                },\n                \"op\": {\n                  \"type\": \"string\",\n                  \"description\": \"The comparison operator.\"\n                },\n                \"values\": {\n                  \"type\": \"array\",\n                  \"description\": \"The values to compare against.\",\n   \
  \               \"items\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          },\n          \"variant\": {\n            \"type\": \"string\",\n            \"description\": \"The variant key to assign when this segment matches.\"\n          },\n          \"percentage\": {\n            \"type\": \"integer\",\n            \"description\": \"The percentage of matching users to include (0-100).\",\n            \"minimum\": 0,\n            \"maximum\": 100\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-update-experiment-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UpdateExperimentRequest
---

---
description: CreateExperimentRequest schema from Amplitude Experiment Management API
layout: schema
name: CreateExperimentRequest
properties_list:
- description: The unique key for the experiment.
  name: key
  type: string
- description: The display name of the experiment.
  name: name
  type: string
- description: A description of the experiment.
  name: description
  type: string
- description: Array of variant configurations.
  name: variants
  type: array
- description: The property used for bucketing.
  name: bucketingKey
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-create-experiment-request-schema.json
slug: experiment-management-api-create-experiment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-create-experiment-request-schema.json\",\n  \"title\": \"CreateExperimentRequest\",\n  \"description\": \"CreateExperimentRequest schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique key for the experiment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the experiment.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the experiment.\"\n    },\n    \"variants\": {\n      \"type\": \"array\",\n      \"description\": \"Array of variant configurations.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n\
  \            \"type\": \"string\",\n            \"description\": \"The unique key for the variant.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the variant.\"\n          },\n          \"payload\": {\n            \"description\": \"An optional JSON payload associated with the variant.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of what this variant does.\"\n          },\n          \"rolloutWeight\": {\n            \"type\": \"integer\",\n            \"description\": \"The rollout weight as a percentage (0-100) controlling traffic allocation to this variant.\",\n            \"minimum\": 0,\n            \"maximum\": 100\n          }\n        }\n      }\n    },\n    \"bucketingKey\": {\n      \"type\": \"string\",\n      \"description\": \"The property used for bucketing.\"\n    }\n  },\n  \"required\": [\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-create-experiment-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: CreateExperimentRequest
---

---
description: ExperimentListResponse schema from Amplitude Experiment Management API
layout: schema
name: ExperimentListResponse
properties_list:
- description: Array of experiment objects.
  name: experiments
  type: array
- description: A cursor for fetching the next page.
  name: nextCursor
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-experiment-list-response-schema.json
slug: experiment-management-api-experiment-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-experiment-list-response-schema.json\",\n  \"title\": \"ExperimentListResponse\",\n  \"description\": \"ExperimentListResponse schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"experiments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of experiment objects.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the experiment.\"\n          },\n          \"projectId\": {\n            \"type\": \"string\",\n            \"description\": \"The project ID the experiment belongs to.\"\n          },\n          \"key\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The unique key used to reference the experiment in code.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the experiment.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of the experiment's purpose.\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the experiment is enabled.\"\n          },\n          \"evaluationMode\": {\n            \"type\": \"string\",\n            \"description\": \"The evaluation mode, either local or remote.\",\n            \"enum\": [\n              \"local\",\n              \"remote\"\n            ]\n          },\n          \"bucketingKey\": {\n            \"type\": \"string\",\n            \"description\": \"The property used for bucketing.\"\n          },\n          \"bucketingSalt\": {\n            \"type\": \"string\",\n          \
  \  \"description\": \"The salt used for hashing.\"\n          },\n          \"variants\": {\n            \"type\": \"array\",\n            \"description\": \"Array of variant configurations including control and treatment groups.\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/VariantConfig\"\n            }\n          },\n          \"deployments\": {\n            \"type\": \"array\",\n            \"description\": \"Array of deployment IDs.\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"segments\": {\n            \"type\": \"array\",\n            \"description\": \"Array of targeting segments.\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Segment\"\n            }\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"description\": \"The current state of the experiment.\",\n            \"enum\": [\n              \"draft\",\n           \
  \   \"running\",\n              \"stopped\",\n              \"archived\"\n            ]\n          },\n          \"rolledOutVariant\": {\n            \"type\": \"string\",\n            \"description\": \"The variant key that was rolled out, if the experiment has concluded.\"\n          },\n          \"startDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the experiment started running.\"\n          },\n          \"endDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the experiment stopped running.\"\n          }\n        }\n      }\n    },\n    \"nextCursor\": {\n      \"type\": \"string\",\n      \"description\": \"A cursor for fetching the next page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-experiment-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: ExperimentListResponse
---

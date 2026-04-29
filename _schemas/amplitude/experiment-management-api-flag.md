---
description: Flag schema from Amplitude Experiment Management API
layout: schema
name: Flag
properties_list:
- description: The unique identifier for the flag.
  name: id
  type: string
- description: The project ID the flag belongs to.
  name: projectId
  type: string
- description: The unique key used to reference the flag in code.
  name: key
  type: string
- description: The display name of the flag.
  name: name
  type: string
- description: A description of the flag's purpose.
  name: description
  type: string
- description: Whether the flag is enabled.
  name: enabled
  type: boolean
- description: The evaluation mode, either local or remote.
  name: evaluationMode
  type: string
- description: The property used for bucketing users into variants.
  name: bucketingKey
  type: string
- description: The salt used for hashing during bucketing.
  name: bucketingSalt
  type: string
- description: Array of variant configurations.
  name: variants
  type: array
- description: Array of deployment IDs the flag is deployed to.
  name: deployments
  type: array
- description: Array of targeting segment configurations.
  name: segments
  type: array
- description: The current state of the flag.
  name: state
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-flag-schema.json
slug: experiment-management-api-flag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-flag-schema.json\",\n  \"title\": \"Flag\",\n  \"description\": \"Flag schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the flag.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The project ID the flag belongs to.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique key used to reference the flag in code.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the flag.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the flag's purpose.\"\n    },\n    \"enabled\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the flag is enabled.\"\n    },\n    \"evaluationMode\": {\n      \"type\": \"string\",\n      \"description\": \"The evaluation mode, either local or remote.\",\n      \"enum\": [\n        \"local\",\n        \"remote\"\n      ]\n    },\n    \"bucketingKey\": {\n      \"type\": \"string\",\n      \"description\": \"The property used for bucketing users into variants.\"\n    },\n    \"bucketingSalt\": {\n      \"type\": \"string\",\n      \"description\": \"The salt used for hashing during bucketing.\"\n    },\n    \"variants\": {\n      \"type\": \"array\",\n      \"description\": \"Array of variant configurations.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"The unique key for the variant.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"\
  The display name of the variant.\"\n          },\n          \"payload\": {\n            \"description\": \"An optional JSON payload associated with the variant.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of what this variant does.\"\n          },\n          \"rolloutWeight\": {\n            \"type\": \"integer\",\n            \"description\": \"The rollout weight as a percentage (0-100) controlling traffic allocation to this variant.\",\n            \"minimum\": 0,\n            \"maximum\": 100\n          }\n        }\n      }\n    },\n    \"deployments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of deployment IDs the flag is deployed to.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of targeting segment configurations.\",\n      \"items\": {\n        \"type\": \"object\",\n    \
  \    \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the segment.\"\n          },\n          \"conditions\": {\n            \"type\": \"array\",\n            \"description\": \"Array of targeting conditions that define this segment.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"description\": \"The condition type.\"\n                },\n                \"prop\": {\n                  \"type\": \"string\",\n                  \"description\": \"The property to evaluate.\"\n                },\n                \"op\": {\n                  \"type\": \"string\",\n                  \"description\": \"The comparison operator.\"\n                },\n                \"values\": {\n                  \"type\": \"array\",\n                  \"description\": \"The values to compare\
  \ against.\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          },\n          \"variant\": {\n            \"type\": \"string\",\n            \"description\": \"The variant key to assign when this segment matches.\"\n          },\n          \"percentage\": {\n            \"type\": \"integer\",\n            \"description\": \"The percentage of matching users to include (0-100).\",\n            \"minimum\": 0,\n            \"maximum\": 100\n          }\n        }\n      }\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the flag.\",\n      \"enum\": [\n        \"draft\",\n        \"active\",\n        \"archived\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-flag-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: Flag
---

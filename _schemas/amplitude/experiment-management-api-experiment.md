---
description: Experiment schema from Amplitude Experiment Management API
layout: schema
name: Experiment
properties_list:
- description: The unique identifier for the experiment.
  name: id
  type: string
- description: The project ID the experiment belongs to.
  name: projectId
  type: string
- description: The unique key used to reference the experiment in code.
  name: key
  type: string
- description: The display name of the experiment.
  name: name
  type: string
- description: A description of the experiment's purpose.
  name: description
  type: string
- description: Whether the experiment is enabled.
  name: enabled
  type: boolean
- description: The evaluation mode, either local or remote.
  name: evaluationMode
  type: string
- description: The property used for bucketing.
  name: bucketingKey
  type: string
- description: The salt used for hashing.
  name: bucketingSalt
  type: string
- description: Array of variant configurations including control and treatment groups.
  name: variants
  type: array
- description: Array of deployment IDs.
  name: deployments
  type: array
- description: Array of targeting segments.
  name: segments
  type: array
- description: The current state of the experiment.
  name: state
  type: string
- description: The variant key that was rolled out, if the experiment has concluded.
  name: rolledOutVariant
  type: string
- description: The date and time the experiment started running.
  name: startDate
  type: string
- description: The date and time the experiment stopped running.
  name: endDate
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-experiment-schema.json
slug: experiment-management-api-experiment
source_filename: experiment-management-api-experiment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-experiment-schema.json\",\n  \"title\": \"Experiment\",\n  \"description\": \"Experiment schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the experiment.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The project ID the experiment belongs to.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique key used to reference the experiment in code.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the experiment.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the\
  \ experiment's purpose.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the experiment is enabled.\"\n    },\n    \"evaluationMode\": {\n      \"type\": \"string\",\n      \"description\": \"The evaluation mode, either local or remote.\",\n      \"enum\": [\n        \"local\",\n        \"remote\"\n      ]\n    },\n    \"bucketingKey\": {\n      \"type\": \"string\",\n      \"description\": \"The property used for bucketing.\"\n    },\n    \"bucketingSalt\": {\n      \"type\": \"string\",\n      \"description\": \"The salt used for hashing.\"\n    },\n    \"variants\": {\n      \"type\": \"array\",\n      \"description\": \"Array of variant configurations including control and treatment groups.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"The unique key for the variant.\"\n          },\n          \"name\": {\n        \
  \    \"type\": \"string\",\n            \"description\": \"The display name of the variant.\"\n          },\n          \"payload\": {\n            \"description\": \"An optional JSON payload associated with the variant.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of what this variant does.\"\n          },\n          \"rolloutWeight\": {\n            \"type\": \"integer\",\n            \"description\": \"The rollout weight as a percentage (0-100) controlling traffic allocation to this variant.\",\n            \"minimum\": 0,\n            \"maximum\": 100\n          }\n        }\n      }\n    },\n    \"deployments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of deployment IDs.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of targeting segments.\",\n      \"items\": {\n        \"type\"\
  : \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the segment.\"\n          },\n          \"conditions\": {\n            \"type\": \"array\",\n            \"description\": \"Array of targeting conditions that define this segment.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"description\": \"The condition type.\"\n                },\n                \"prop\": {\n                  \"type\": \"string\",\n                  \"description\": \"The property to evaluate.\"\n                },\n                \"op\": {\n                  \"type\": \"string\",\n                  \"description\": \"The comparison operator.\"\n                },\n                \"values\": {\n                  \"type\": \"array\",\n                  \"description\": \"The\
  \ values to compare against.\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          },\n          \"variant\": {\n            \"type\": \"string\",\n            \"description\": \"The variant key to assign when this segment matches.\"\n          },\n          \"percentage\": {\n            \"type\": \"integer\",\n            \"description\": \"The percentage of matching users to include (0-100).\",\n            \"minimum\": 0,\n            \"maximum\": 100\n          }\n        }\n      }\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the experiment.\",\n      \"enum\": [\n        \"draft\",\n        \"running\",\n        \"stopped\",\n        \"archived\"\n      ]\n    },\n    \"rolledOutVariant\": {\n      \"type\": \"string\",\n      \"description\": \"The variant key that was rolled out, if the experiment has concluded.\"\n\
  \    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the experiment started running.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the experiment stopped running.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-experiment-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: Experiment
---

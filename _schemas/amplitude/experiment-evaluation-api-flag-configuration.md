---
description: FlagConfiguration schema from Amplitude Experiment Evaluation API
layout: schema
name: FlagConfiguration
properties_list:
- description: The unique key identifying the flag.
  name: key
  type: string
- description: Metadata about the flag configuration.
  name: metadata
  type: object
- description: Array of targeting segments for this flag.
  name: segments
  type: array
- description: Map of variant keys to variant configuration objects.
  name: variants
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-evaluation-api-flag-configuration-schema.json
slug: experiment-evaluation-api-flag-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-evaluation-api-flag-configuration-schema.json\",\n  \"title\": \"FlagConfiguration\",\n  \"description\": \"FlagConfiguration schema from Amplitude Experiment Evaluation API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique key identifying the flag.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the flag configuration.\",\n      \"properties\": {\n        \"deployed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the flag is currently deployed.\"\n        },\n        \"evaluationMode\": {\n          \"type\": \"string\",\n          \"description\": \"The evaluation mode, either local or remote.\"\n        },\n        \"flagType\": {\n \
  \         \"type\": \"string\",\n          \"description\": \"The type of flag, such as experiment or release.\"\n        },\n        \"flagVersion\": {\n          \"type\": \"integer\",\n          \"description\": \"The version of the flag configuration.\"\n        }\n      }\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of targeting segments for this flag.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"conditions\": {\n            \"type\": \"array\",\n            \"description\": \"Array of targeting conditions.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"additionalProperties\": true\n            }\n          },\n          \"variant\": {\n            \"type\": \"string\",\n            \"description\": \"The variant key to assign when conditions are met.\"\n          }\n        }\n      }\n    },\n    \"variants\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Map of variant keys to variant configuration objects.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"The variant key.\"\n          },\n          \"payload\": {\n            \"description\": \"Optional payload for the variant.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-evaluation-api-flag-configuration-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: FlagConfiguration
---

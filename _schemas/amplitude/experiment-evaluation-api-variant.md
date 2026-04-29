---
description: Variant schema from Amplitude Experiment Evaluation API
layout: schema
name: Variant
properties_list:
- description: The variant key identifying this variant.
  name: key
  type: string
- description: The variant value or payload.
  name: value
  type: string
- description: An optional JSON payload associated with the variant.
  name: payload
  type: object
- description: Metadata about the variant assignment.
  name: metadata
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-evaluation-api-variant-schema.json
slug: experiment-evaluation-api-variant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-evaluation-api-variant-schema.json\",\n  \"title\": \"Variant\",\n  \"description\": \"Variant schema from Amplitude Experiment Evaluation API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The variant key identifying this variant.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The variant value or payload.\"\n    },\n    \"payload\": {\n      \"description\": \"An optional JSON payload associated with the variant.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the variant assignment.\",\n      \"properties\": {\n        \"experimentKey\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the experiment that assigned\
  \ this variant.\"\n        },\n        \"flagType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of flag, such as experiment or release.\"\n        },\n        \"flagVersion\": {\n          \"type\": \"integer\",\n          \"description\": \"The version of the flag configuration.\"\n        },\n        \"default\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is the default variant.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-evaluation-api-variant-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: Variant
---

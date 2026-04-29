---
description: VariantConfig schema from Amplitude Experiment Management API
layout: schema
name: VariantConfig
properties_list:
- description: The unique key for the variant.
  name: key
  type: string
- description: The display name of the variant.
  name: name
  type: string
- description: An optional JSON payload associated with the variant.
  name: payload
  type: object
- description: A description of what this variant does.
  name: description
  type: string
- description: The rollout weight as a percentage (0-100) controlling traffic allocation to this variant.
  name: rolloutWeight
  type: integer
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-variant-config-schema.json
slug: experiment-management-api-variant-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-variant-config-schema.json\",\n  \"title\": \"VariantConfig\",\n  \"description\": \"VariantConfig schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique key for the variant.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the variant.\"\n    },\n    \"payload\": {\n      \"description\": \"An optional JSON payload associated with the variant.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what this variant does.\"\n    },\n    \"rolloutWeight\": {\n      \"type\": \"integer\",\n      \"description\": \"The rollout weight as a percentage (0-100) controlling\
  \ traffic allocation to this variant.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-variant-config-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: VariantConfig
---

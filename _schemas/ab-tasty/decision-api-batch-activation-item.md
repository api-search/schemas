---
description: BatchActivationItem schema from AB Tasty Decision API
layout: schema
name: BatchActivationItem
properties_list:
- description: Visitor ID
  name: vid
  type: string
- description: Variation group ID
  name: caid
  type: string
- description: Variation ID
  name: vaid
  type: string
- description: Time delta in milliseconds for offline/latent hits (0-4 hours)
  name: qt
  type: integer
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-batch-activation-item-schema.json
slug: decision-api-batch-activation-item
source_filename: decision-api-batch-activation-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-batch-activation-item-schema.json\",\n  \"title\": \"BatchActivationItem\",\n  \"description\": \"BatchActivationItem schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vid\": {\n      \"type\": \"string\",\n      \"description\": \"Visitor ID\",\n      \"example\": \"user123\"\n    },\n    \"caid\": {\n      \"type\": \"string\",\n      \"description\": \"Variation group ID\",\n      \"example\": \"vg_123\"\n    },\n    \"vaid\": {\n      \"type\": \"string\",\n      \"description\": \"Variation ID\",\n      \"example\": \"var_456\"\n    },\n    \"qt\": {\n      \"type\": \"integer\",\n      \"description\": \"Time delta in milliseconds for offline/latent hits (0-4 hours)\",\n      \"minimum\": 0,\n      \"example\": 2134\n    }\n  },\n  \"required\": [\n \
  \   \"vid\",\n    \"caid\",\n    \"vaid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-batch-activation-item-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: BatchActivationItem
---

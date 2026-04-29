---
description: FlagMetadata schema from AB Tasty Decision API
layout: schema
name: FlagMetadata
properties_list:
- description: Campaign ID
  name: campaignId
  type: string
- description: Campaign name
  name: campaignName
  type: string
- description: Campaign slug (if configured)
  name: slug
  type: string
- description: Campaign type
  name: type
  type: string
- description: Variation group ID
  name: variationGroupId
  type: string
- description: Variation group name
  name: variationGroupName
  type: string
- description: Variation ID
  name: variationId
  type: string
- description: Variation name
  name: variationName
  type: string
- description: Indicates if the variation is a reference variation
  name: reference
  type: boolean
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-flag-metadata-schema.json
slug: decision-api-flag-metadata
source_filename: decision-api-flag-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-flag-metadata-schema.json\",\n  \"title\": \"FlagMetadata\",\n  \"description\": \"FlagMetadata schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign ID\",\n      \"example\": \"campaign_abc\"\n    },\n    \"campaignName\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign name\",\n      \"example\": \"New Checkout Experiment\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Campaign slug (if configured)\",\n      \"example\": \"checkout-exp\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign type\",\n      \"example\": \"ab\"\n    },\n    \"variationGroupId\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Variation group ID\",\n      \"example\": \"vg_123\"\n    },\n    \"variationGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"Variation group name\",\n      \"example\": \"Variation Group A\"\n    },\n    \"variationId\": {\n      \"type\": \"string\",\n      \"description\": \"Variation ID\",\n      \"example\": \"var_456\"\n    },\n    \"variationName\": {\n      \"type\": \"string\",\n      \"description\": \"Variation name\",\n      \"example\": \"Treatment\"\n    },\n    \"reference\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the variation is a reference variation\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-flag-metadata-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: FlagMetadata
---

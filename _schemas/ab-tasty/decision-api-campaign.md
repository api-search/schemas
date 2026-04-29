---
description: Campaign schema from AB Tasty Decision API
layout: schema
name: Campaign
properties_list:
- description: Campaign ID
  name: id
  type: string
- description: Variation group ID (corresponds to a scenario in Flagship)
  name: variationGroupId
  type: string
- description: ''
  name: variation
  type: object
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-campaign-schema.json
slug: decision-api-campaign
source_filename: decision-api-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-schema.json\",\n  \"title\": \"Campaign\",\n  \"description\": \"Campaign schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign ID\",\n      \"example\": \"campaign_abc\"\n    },\n    \"variationGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"Variation group ID (corresponds to a scenario in Flagship)\",\n      \"example\": \"vg_123\"\n    },\n    \"variation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Variation ID\",\n          \"example\": \"var_456\"\n        },\n        \"modifications\": {\n          \"type\": \"object\",\n          \"properties\": {\n          \
  \  \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"NULL\",\n                \"JSON\",\n                \"TEXT\",\n                \"IMAGE\",\n                \"HTML\",\n                \"FLAG\",\n                \"REDIRECT\"\n              ],\n              \"description\": \"The modification type\"\n            },\n            \"value\": {\n              \"oneOf\": [\n                {\n                  \"type\": \"object\"\n                },\n                {\n                  \"type\": \"string\"\n                }\n              ],\n              \"description\": \"The value of the modification (structure depends on type)\",\n              \"example\": {\n                \"button_color\": \"blue\",\n                \"feature_enabled\": true\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: Campaign
---

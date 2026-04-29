---
description: CampaignVariation schema from AB Tasty Decision API
layout: schema
name: CampaignVariation
properties_list:
- description: ''
  name: campaignId
  type: string
- description: ''
  name: variationId
  type: string
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-campaign-variation-schema.json
slug: decision-api-campaign-variation
source_filename: decision-api-campaign-variation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-variation-schema.json\",\n  \"title\": \"CampaignVariation\",\n  \"description\": \"CampaignVariation schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"example\": \"campaign_abc\"\n    },\n    \"variationId\": {\n      \"type\": \"string\",\n      \"example\": \"var_456\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-variation-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: CampaignVariation
---

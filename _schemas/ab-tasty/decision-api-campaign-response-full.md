---
description: CampaignResponseFull schema from AB Tasty Decision API
layout: schema
name: CampaignResponseFull
properties_list:
- description: ''
  name: visitorId
  type: string
- description: ''
  name: campaigns
  type: array
- description: ''
  name: campaignsVariation
  type: array
- description: ''
  name: mergedModifications
  type: object
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-campaign-response-full-schema.json
slug: decision-api-campaign-response-full
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-response-full-schema.json\",\n  \"title\": \"CampaignResponseFull\",\n  \"description\": \"CampaignResponseFull schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"visitorId\": {\n      \"type\": \"string\",\n      \"example\": \"user123\"\n    },\n    \"campaigns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Campaign\"\n      }\n    },\n    \"campaignsVariation\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CampaignVariation\"\n      }\n    },\n    \"mergedModifications\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-response-full-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: CampaignResponseFull
---

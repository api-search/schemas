---
description: CampaignResponseSimple schema from AB Tasty Decision API
layout: schema
name: CampaignResponseSimple
properties_list:
- description: ''
  name: campaignsVariation
  type: array
- description: All remote values merged into a single object
  name: mergedModifications
  type: object
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-campaign-response-simple-schema.json
slug: decision-api-campaign-response-simple
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-response-simple-schema.json\",\n  \"title\": \"CampaignResponseSimple\",\n  \"description\": \"CampaignResponseSimple schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignsVariation\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CampaignVariation\"\n      }\n    },\n    \"mergedModifications\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"All remote values merged into a single object\",\n      \"example\": {\n        \"button_color\": \"blue\",\n        \"feature_enabled\": true,\n        \"welcome_text\": \"Hello!\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-response-simple-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: CampaignResponseSimple
---

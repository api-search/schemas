---
description: CampaignResponseNormal schema from AB Tasty Decision API
layout: schema
name: CampaignResponseNormal
properties_list:
- description: ''
  name: visitorId
  type: string
- description: ''
  name: campaigns
  type: array
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-campaign-response-normal-schema.json
slug: decision-api-campaign-response-normal
source_filename: decision-api-campaign-response-normal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-response-normal-schema.json\",\n  \"title\": \"CampaignResponseNormal\",\n  \"description\": \"CampaignResponseNormal schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"visitorId\": {\n      \"type\": \"string\",\n      \"example\": \"user123\"\n    },\n    \"campaigns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Campaign\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-response-normal-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: CampaignResponseNormal
---

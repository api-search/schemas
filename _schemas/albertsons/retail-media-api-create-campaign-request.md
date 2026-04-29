---
description: Request body for creating a new advertising campaign.
layout: schema
name: Create Campaign Request
properties_list:
- description: Display name for the new campaign.
  name: name
  type: string
- description: Total budget allocated to the campaign in USD.
  name: budget
  type: number
- description: Campaign start date (ISO 8601).
  name: startDate
  type: string
- description: Campaign end date (ISO 8601).
  name: endDate
  type: string
- description: List of audience segment IDs for targeting.
  name: targetAudienceIds
  type: array
provider_name: albertsons
provider_slug: albertsons
schema_file: json-schema/retail-media-api-create-campaign-request-schema.json
slug: retail-media-api-create-campaign-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-create-campaign-request-schema.json\",\n  \"title\": \"Create Campaign Request\",\n  \"description\": \"Request body for creating a new advertising campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the new campaign.\",\n      \"example\": \"Summer Grocery Promotion\"\n    },\n    \"budget\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total budget allocated to the campaign in USD.\",\n      \"example\": 25000.0\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Campaign start date (ISO 8601).\",\n      \"example\": \"2026-06-01\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n \
  \     \"format\": \"date\",\n      \"description\": \"Campaign end date (ISO 8601).\",\n      \"example\": \"2026-08-31\"\n    },\n    \"targetAudienceIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of audience segment IDs for targeting.\",\n      \"example\": [\n        \"aud-001\",\n        \"aud-002\"\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"budget\",\n    \"startDate\",\n    \"endDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-create-campaign-request-schema.json
tags:
- Grocery
- Retail
- Retail Media
- Advertising
- Campaigns
- Analytics
- Consumer Goods
- Food
- Pharmacy
title: Create Campaign Request
---

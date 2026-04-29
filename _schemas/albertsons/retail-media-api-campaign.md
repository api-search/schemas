---
description: An advertising campaign on the Albertsons Media Collective platform.
layout: schema
name: Campaign
properties_list:
- description: Unique identifier of the campaign.
  name: campaignId
  type: string
- description: Display name of the campaign.
  name: name
  type: string
- description: Current status of the campaign.
  name: status
  type: string
- description: Total budget allocated to the campaign in USD.
  name: budget
  type: number
- description: Campaign start date in ISO 8601 format.
  name: startDate
  type: string
- description: Campaign end date in ISO 8601 format.
  name: endDate
  type: string
- description: Total impressions delivered for the campaign.
  name: impressions
  type: integer
- description: Total clicks recorded for the campaign.
  name: clicks
  type: integer
provider_name: albertsons
provider_slug: albertsons
schema_file: json-schema/retail-media-api-campaign-schema.json
slug: retail-media-api-campaign
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-campaign-schema.json\",\n  \"title\": \"Campaign\",\n  \"description\": \"An advertising campaign on the Albertsons Media Collective platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the campaign.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the campaign.\",\n      \"example\": \"Spring Grocery Promotion\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"paused\",\n        \"completed\",\n        \"draft\"\n      ],\n      \"description\": \"Current status of the campaign.\",\n      \"example\": \"active\"\n    },\n    \"budget\": {\n      \"type\"\
  : \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total budget allocated to the campaign in USD.\",\n      \"example\": 50000.0\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Campaign start date in ISO 8601 format.\",\n      \"example\": \"2026-03-01\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Campaign end date in ISO 8601 format.\",\n      \"example\": \"2026-05-31\"\n    },\n    \"impressions\": {\n      \"type\": \"integer\",\n      \"description\": \"Total impressions delivered for the campaign.\",\n      \"example\": 1250000\n    },\n    \"clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Total clicks recorded for the campaign.\",\n      \"example\": 18750\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-campaign-schema.json
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
title: Campaign
---

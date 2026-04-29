---
description: Schema for a Google Ads campaign managed by Blobr AI platform
layout: schema
name: Blobr Campaign
properties_list:
- description: Google Ads campaign ID
  name: campaignId
  type: string
- description: Campaign name
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: Campaign channel type
  name: advertisingChannelType
  type: string
- description: ''
  name: budget
  type: object
- description: ''
  name: biddingStrategy
  type: object
- description: ''
  name: metrics
  type: object
provider_name: Blobr
provider_slug: blobr
schema_file: json-schema/blobr-campaign-schema.json
slug: blobr-campaign
source_filename: blobr-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blobr/main/json-schema/blobr-campaign-schema.json\",\n  \"title\": \"Blobr Campaign\",\n  \"description\": \"Schema for a Google Ads campaign managed by Blobr AI platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignId\": { \"type\": \"string\", \"description\": \"Google Ads campaign ID\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Campaign name\" },\n    \"status\": { \"type\": \"string\", \"enum\": [\"ENABLED\", \"PAUSED\", \"REMOVED\"] },\n    \"advertisingChannelType\": {\n      \"type\": \"string\",\n      \"enum\": [\"SEARCH\", \"DISPLAY\", \"SHOPPING\", \"VIDEO\", \"SMART\", \"PERFORMANCE_MAX\"],\n      \"description\": \"Campaign channel type\"\n    },\n    \"budget\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amountMicros\": { \"type\": \"integer\", \"description\": \"Daily budget\
  \ in micros (1M = $1)\" },\n        \"deliveryMethod\": { \"type\": \"string\", \"enum\": [\"STANDARD\", \"ACCELERATED\"] }\n      }\n    },\n    \"biddingStrategy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"TARGET_CPA\", \"TARGET_ROAS\", \"MAXIMIZE_CONVERSIONS\", \"MAXIMIZE_CONVERSION_VALUE\", \"TARGET_IMPRESSION_SHARE\", \"MANUAL_CPC\"]\n        },\n        \"targetCpaMicros\": { \"type\": \"integer\" },\n        \"targetRoas\": { \"type\": \"number\" }\n      }\n    },\n    \"metrics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"impressions\": { \"type\": \"integer\" },\n        \"clicks\": { \"type\": \"integer\" },\n        \"costMicros\": { \"type\": \"integer\" },\n        \"conversions\": { \"type\": \"number\" },\n        \"ctr\": { \"type\": \"number\" },\n        \"averageCpc\": { \"type\": \"number\" },\n        \"conversionRate\": { \"type\": \"number\" },\n\
  \        \"roas\": { \"type\": \"number\" }\n      }\n    }\n  },\n  \"required\": [\"campaignId\", \"name\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blobr/refs/heads/main/json-schema/blobr-campaign-schema.json
tags:
- Advertising
- AI Agents
- Google Ads
- Marketing Automation
- PPC
title: Blobr Campaign
---

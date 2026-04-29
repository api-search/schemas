---
description: Campaign schema from Amazon Advertising API
layout: schema
name: Campaign
properties_list:
- description: ''
  name: campaignId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: dailyBudget
  type: number
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: targetingType
  type: string
- description: ''
  name: premiumBidAdjustment
  type: boolean
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/advertising-campaign-schema.json
slug: advertising-campaign
source_filename: advertising-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"enabled\",\n        \"paused\",\n        \"archived\"\n      ]\n    },\n    \"dailyBudget\": {\n      \"type\": \"number\"\n    },\n    \"startDate\": {\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"type\": \"string\"\n    },\n    \"targetingType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"manual\",\n        \"auto\"\n      ]\n    },\n    \"premiumBidAdjustment\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Campaign\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-campaign-schema.json\",\n  \"description\": \"Campaign schema from Amazon Advertising API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-campaign-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Campaign
---

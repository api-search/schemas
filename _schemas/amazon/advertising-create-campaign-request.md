---
description: CreateCampaignRequest schema from Amazon Advertising API
layout: schema
name: CreateCampaignRequest
properties_list:
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
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/advertising-create-campaign-request-schema.json
slug: advertising-create-campaign-request
source_filename: advertising-create-campaign-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"state\",\n    \"dailyBudget\",\n    \"startDate\",\n    \"targetingType\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"enabled\",\n        \"paused\"\n      ]\n    },\n    \"dailyBudget\": {\n      \"type\": \"number\"\n    },\n    \"startDate\": {\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"type\": \"string\"\n    },\n    \"targetingType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"manual\",\n        \"auto\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCampaignRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-create-campaign-request-schema.json\",\n  \"description\": \"CreateCampaignRequest schema from Amazon Advertising API\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-create-campaign-request-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: CreateCampaignRequest
---

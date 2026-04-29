---
description: Target schema from Amazon Advertising API
layout: schema
name: Target
properties_list:
- description: ''
  name: targetId
  type: string
- description: ''
  name: campaignId
  type: string
- description: ''
  name: adGroupId
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: bid
  type: number
- description: ''
  name: expressionType
  type: string
- description: ''
  name: expression
  type: array
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/advertising-target-schema.json
slug: advertising-target
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetId\": {\n      \"type\": \"string\"\n    },\n    \"campaignId\": {\n      \"type\": \"string\"\n    },\n    \"adGroupId\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"bid\": {\n      \"type\": \"number\"\n    },\n    \"expressionType\": {\n      \"type\": \"string\"\n    },\n    \"expression\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Target\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-target-schema.json\",\n  \"description\": \"Target schema from Amazon Advertising API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-target-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Target
---

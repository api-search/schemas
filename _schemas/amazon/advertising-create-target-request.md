---
description: CreateTargetRequest schema from Amazon Advertising API
layout: schema
name: CreateTargetRequest
properties_list:
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
  name: expression
  type: array
- description: ''
  name: expressionType
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/advertising-create-target-request-schema.json
slug: advertising-create-target-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"campaignId\",\n    \"adGroupId\",\n    \"state\",\n    \"expression\",\n    \"expressionType\"\n  ],\n  \"properties\": {\n    \"campaignId\": {\n      \"type\": \"string\"\n    },\n    \"adGroupId\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"bid\": {\n      \"type\": \"number\"\n    },\n    \"expression\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"expressionType\": {\n      \"type\": \"string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTargetRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-create-target-request-schema.json\",\n  \"description\": \"CreateTargetRequest schema from Amazon Advertising API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-create-target-request-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: CreateTargetRequest
---

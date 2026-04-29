---
description: Keyword schema from Amazon Advertising API
layout: schema
name: Keyword
properties_list:
- description: ''
  name: keywordId
  type: string
- description: ''
  name: campaignId
  type: string
- description: ''
  name: adGroupId
  type: string
- description: ''
  name: keywordText
  type: string
- description: ''
  name: matchType
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: bid
  type: number
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/advertising-keyword-schema.json
slug: advertising-keyword
source_filename: advertising-keyword-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"keywordId\": {\n      \"type\": \"string\"\n    },\n    \"campaignId\": {\n      \"type\": \"string\"\n    },\n    \"adGroupId\": {\n      \"type\": \"string\"\n    },\n    \"keywordText\": {\n      \"type\": \"string\"\n    },\n    \"matchType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"broad\",\n        \"exact\",\n        \"phrase\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"bid\": {\n      \"type\": \"number\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Keyword\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-keyword-schema.json\",\n  \"description\": \"Keyword schema from Amazon Advertising API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-keyword-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Keyword
---

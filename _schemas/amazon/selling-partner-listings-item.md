---
description: ListingsItem schema from Amazon Selling Partner API
layout: schema
name: ListingsItem
properties_list:
- description: ''
  name: sku
  type: string
- description: ''
  name: summaries
  type: array
- description: ''
  name: attributes
  type: object
- description: ''
  name: issues
  type: array
- description: ''
  name: offers
  type: array
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-listings-item-schema.json
slug: selling-partner-listings-item
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"sku\": {\n      \"type\": \"string\"\n    },\n    \"summaries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"attributes\": {\n      \"type\": \"object\"\n    },\n    \"issues\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"offers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListingsItem\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-listings-item-schema.json\",\n  \"description\": \"ListingsItem schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-listings-item-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: ListingsItem
---

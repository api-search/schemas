---
description: CatalogItem schema from Amazon Selling Partner API
layout: schema
name: CatalogItem
properties_list:
- description: ''
  name: asin
  type: string
- description: ''
  name: attributes
  type: object
- description: ''
  name: images
  type: array
- description: ''
  name: salesRanks
  type: array
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-catalog-item-schema.json
slug: selling-partner-catalog-item
source_filename: selling-partner-catalog-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"asin\": {\n      \"type\": \"string\"\n    },\n    \"attributes\": {\n      \"type\": \"object\"\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"salesRanks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CatalogItem\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-catalog-item-schema.json\",\n  \"description\": \"CatalogItem schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-catalog-item-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: CatalogItem
---

---
description: CatalogItemList schema from Amazon Selling Partner API
layout: schema
name: CatalogItemList
properties_list:
- description: ''
  name: numberOfResults
  type: integer
- description: ''
  name: pagination
  type: object
- description: ''
  name: items
  type: array
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-catalog-item-list-schema.json
slug: selling-partner-catalog-item-list
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"numberOfResults\": {\n      \"type\": \"integer\"\n    },\n    \"pagination\": {\n      \"$ref\": \"#/components/schemas/Pagination\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CatalogItem\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CatalogItemList\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-catalog-item-list-schema.json\",\n  \"description\": \"CatalogItemList schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-catalog-item-list-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: CatalogItemList
---

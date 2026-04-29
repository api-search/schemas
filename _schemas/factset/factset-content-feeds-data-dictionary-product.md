---
description: ''
layout: schema
name: Product
properties_list:
- description: Unique identifier for the product
  name: id
  type: string
- description: Name of the product
  name: name
  type: string
- description: URL to the product page on the Open:FactSet Marketplace
  name: ofmLink
  type: string
- description: The id defining a product in the Open:FactSet Marketplace
  name: ofmProductId
  type: string
- description: Flag indicating if the user is entitled to access the data in their subscriptions
  name: entitled
  type: boolean
- description: Name of the Data Provider for the product
  name: providerName
  type: string
- description: Flag indicating if this product is available in a data feed
  name: dataFeed
  type: boolean
- description: Flag indicating if this product is available in an api
  name: api
  type: boolean
- description: Flag indicating if this product is maintained by RDF/UCF
  name: referenceDataFeed
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-content-feeds-data-dictionary-product-schema.json
slug: factset-content-feeds-data-dictionary-product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Product\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the product\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the product\"\n    },\n    \"ofmLink\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the product page on the Open:FactSet Marketplace\"\n    },\n    \"ofmProductId\": {\n      \"type\": \"string\",\n      \"description\": \"The id defining a product in the Open:FactSet Marketplace\"\n    },\n    \"entitled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if the user is entitled to access the data in their subscriptions\"\n    },\n    \"providerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Data Provider for the product\"\n    },\n    \"dataFeed\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Flag indicating if this product is available in a data feed\"\n    },\n    \"api\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if this product is available in an api\"\n    },\n    \"referenceDataFeed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if this product is maintained by RDF/UCF\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-content-feeds-data-dictionary-product-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Product
---

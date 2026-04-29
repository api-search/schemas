---
description: ''
layout: schema
name: DataItem
properties_list:
- description: Unique identifier for the data item
  name: id
  type: integer
- description: Name of the data item
  name: name
  type: string
- description: Description of the data item
  name: description
  type: string
- description: Flag indicating if the user is entitled to access the data in their subscriptions
  name: entitled
  type: boolean
- description: Flag indicating if this item is available in a data feed
  name: dataFeed
  type: boolean
- description: Flag indicating if this item is available in an api
  name: api
  type: boolean
- description: Flag indicating if this product is maintained by RDF/UCF
  name: referenceDataFeed
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-content-feeds-data-dictionary-data-item-schema.json
slug: factset-content-feeds-data-dictionary-data-item
source_filename: factset-content-feeds-data-dictionary-data-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the data item\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the data item\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the data item\"\n    },\n    \"entitled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if the user is entitled to access the data in their subscriptions\"\n    },\n    \"dataFeed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if this item is available in a data feed\"\n    },\n    \"api\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if this item is available in an api\"\n    },\n    \"referenceDataFeed\": {\n      \"type\": \"boolean\",\n\
  \      \"description\": \"Flag indicating if this product is maintained by RDF/UCF\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-content-feeds-data-dictionary-data-item-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: DataItem
---

---
description: ''
layout: schema
name: Merchants
properties_list:
- description: The number of items in the retrieved data set
  name: count
  type: integer
- description: The number of items requested to be retrieved
  name: limit
  type: integer
- description: The page offset used for the query
  name: offset
  type: integer
- description: The total number of merchants available to be retrieved
  name: total
  type: integer
- description: The list of merchants retrieved
  name: merchants
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-merchant-locations-merchants-schema.json
slug: mastercard-merchant-locations-merchants
source_filename: mastercard-merchant-locations-merchants-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Merchants\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the retrieved data set\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items requested to be retrieved\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"The page offset used for the query\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of merchants available to be retrieved\"\n    },\n    \"merchants\": {\n      \"type\": \"array\",\n      \"description\": \"The list of merchants retrieved\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-merchant-locations-merchants-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Merchants
---

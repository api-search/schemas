---
description: ''
layout: schema
name: Atms
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
- description: The total number of ATMs available to be retrieved
  name: total
  type: integer
- description: The list of ATMs retrieved
  name: atms
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-atm-locations-atms-schema.json
slug: mastercard-atm-locations-atms
source_filename: mastercard-atm-locations-atms-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Atms\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the retrieved data set\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items requested to be retrieved\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"The page offset used for the query\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of ATMs available to be retrieved\"\n    },\n    \"atms\": {\n      \"type\": \"array\",\n      \"description\": \"The list of ATMs retrieved\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-atm-locations-atms-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Atms
---

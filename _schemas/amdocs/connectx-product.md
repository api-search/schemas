---
description: Product schema from Amdocs API
layout: schema
name: Product
properties_list:
- description: ''
  name: productId
  type: string
- description: ''
  name: productName
  type: string
- description: ''
  name: productType
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: monthlyPrice
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: features
  type: array
- description: ''
  name: status
  type: string
provider_name: Amdocs
provider_slug: amdocs
schema_file: json-schema/connectx-product-schema.json
slug: connectx-product
source_filename: connectx-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"Product schema from Amdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\"\n    },\n    \"productName\": {\n      \"type\": \"string\"\n    },\n    \"productType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Mobile\",\n        \"Broadband\",\n        \"TV\",\n        \"Bundle\",\n        \"Addon\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"monthlyPrice\": {\n      \"type\": \"number\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"\
  enum\": [\n        \"Active\",\n        \"Discontinued\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/json-schema/connectx-product-schema.json
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
title: Product
---

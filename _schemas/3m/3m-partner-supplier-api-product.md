---
description: A 3M product available to partners and suppliers
layout: schema
name: Product
properties_list:
- description: Unique product identifier
  name: productId
  type: string
- description: Product display name
  name: name
  type: string
- description: Stock Keeping Unit identifier
  name: sku
  type: string
- description: Product category
  name: category
  type: string
- description: Detailed product description
  name: description
  type: string
- description: Unit price for the product
  name: unitPrice
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Product availability status
  name: availability
  type: string
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-product-schema.json
slug: 3m-partner-supplier-api-product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"A 3M product available to partners and suppliers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier\",\n      \"example\": \"PROD-12345\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product display name\",\n      \"example\": \"3M Scotch Heavy Duty Tape\"\n    },\n    \"sku\": {\n      \"type\": \"string\",\n      \"description\": \"Stock Keeping Unit identifier\",\n      \"example\": \"SKU-12345\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category\",\n      \"example\": \"adhesives\"\n    },\n    \"description\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Detailed product description\",\n      \"example\": \"Heavy duty packaging tape for industrial use\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Unit price for the product\",\n      \"example\": 24.99\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\",\n      \"example\": \"USD\"\n    },\n    \"availability\": {\n      \"type\": \"string\",\n      \"description\": \"Product availability status\",\n      \"enum\": [\n        \"in-stock\",\n        \"out-of-stock\",\n        \"limited\",\n        \"discontinued\"\n      ],\n      \"example\": \"in-stock\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-product-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: Product
---

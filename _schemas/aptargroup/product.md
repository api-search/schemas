---
description: A dispensing, sealing, or packaging product from AptarGroup
layout: schema
name: Product
properties_list:
- description: Unique product identifier
  name: productId
  type: string
- description: Product name
  name: name
  type: string
- description: Product category (dispensing, sealing, active-packaging)
  name: category
  type: string
- description: Target market (beauty, pharma, food, home-care, etc.)
  name: market
  type: string
- description: Product description
  name: description
  type: string
- description: Primary material (plastic, aluminum, glass, etc.)
  name: material
  type: string
- description: Whether the product uses sustainable materials
  name: sustainable
  type: boolean
- description: Stock keeping unit identifier
  name: sku
  type: string
provider_name: AptarGroup
provider_slug: aptargroup
schema_file: json-schema/product-schema.json
slug: product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aptargroup/main/json-schema/product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"A dispensing, sealing, or packaging product from AptarGroup\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category (dispensing, sealing, active-packaging)\"\n    },\n    \"market\": {\n      \"type\": \"string\",\n      \"description\": \"Target market (beauty, pharma, food, home-care, etc.)\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description\"\n    },\n    \"material\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Primary material (plastic, aluminum, glass, etc.)\"\n    },\n    \"sustainable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product uses sustainable materials\"\n    },\n    \"sku\": {\n      \"type\": \"string\",\n      \"description\": \"Stock keeping unit identifier\"\n    }\n  },\n  \"required\": [\n    \"productId\",\n    \"name\",\n    \"category\",\n    \"market\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aptargroup/refs/heads/main/json-schema/product-schema.json
tags:
- Packaging
- Dispensing
- Manufacturing
- Sustainability
- Consumer Goods
title: Product
---

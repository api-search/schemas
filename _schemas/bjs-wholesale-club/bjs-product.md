---
description: Schema for a BJ's Wholesale Club product record
layout: schema
name: BJS Product
properties_list:
- description: Unique product identifier
  name: productId
  type: string
- description: Product display name
  name: name
  type: string
- description: Full product description
  name: description
  type: string
- description: ''
  name: brand
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: subcategory
  type: string
- description: Member price in USD
  name: price
  type: number
- description: Regular retail price in USD
  name: regularPrice
  type: number
- description: Unit of measure
  name: unit
  type: string
- description: ''
  name: images
  type: array
- description: ''
  name: memberExclusive
  type: boolean
- description: ''
  name: inStock
  type: boolean
provider_name: BJ's Wholesale Club
provider_slug: bjs-wholesale-club
schema_file: json-schema/bjs-product-schema.json
slug: bjs-product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/main/json-schema/bjs-product-schema.json\",\n  \"title\": \"BJS Product\",\n  \"description\": \"Schema for a BJ's Wholesale Club product record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product display name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full product description\"\n    },\n    \"brand\": {\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"type\": \"string\"\n    },\n    \"subcategory\": {\n      \"type\": \"string\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Member price in USD\"\n    },\n    \"regularPrice\": {\n      \"type\"\
  : \"number\",\n      \"description\": \"Regular retail price in USD\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure\"\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"memberExclusive\": {\n      \"type\": \"boolean\"\n    },\n    \"inStock\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\"productId\", \"name\", \"price\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/refs/heads/main/json-schema/bjs-product-schema.json
tags:
- Ecommerce
- Membership
- Retail
- Wholesale
title: BJS Product
---

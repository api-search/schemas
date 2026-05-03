---
description: A beauty product in the Sally Beauty Holdings product catalog, sold through Sally Beauty Supply or BSG professional distribution channels.
layout: schema
name: Sally Beauty Product
properties_list:
- description: Unique product identifier (SKU)
  name: id
  type: string
- description: Product name
  name: name
  type: string
- description: Brand name
  name: brand
  type: string
- description: Product description
  name: description
  type: string
- description: Product category
  name: category
  type: string
- description: Product subcategory
  name: subcategory
  type: string
- description: Retail price in USD
  name: price
  type: number
- description: Professional (BSG) price for licensed salon professionals
  name: professional_price
  type: number
- description: Currency code
  name: currency
  type: string
- description: Universal Product Code
  name: upc
  type: string
- description: Product image URLs
  name: images
  type: array
- description: Whether product is available for online purchase
  name: available_online
  type: boolean
- description: Whether product is available in physical stores
  name: available_in_store
  type: boolean
- description: Whether product is restricted to licensed professionals (BSG only)
  name: professional_only
  type: boolean
- description: Sales channel
  name: channel
  type: string
- description: ''
  name: ratings
  type: object
provider_name: Sally Beauty Holdings
provider_slug: sally-beauty-holdings
schema_file: json-schema/sally-beauty-product-schema.json
slug: sally-beauty-product
source_filename: sally-beauty-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sally-beauty-holdings/json-schema/sally-beauty-product-schema.json\",\n  \"title\": \"Sally Beauty Product\",\n  \"description\": \"A beauty product in the Sally Beauty Holdings product catalog, sold through Sally Beauty Supply or BSG professional distribution channels.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier (SKU)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Brand name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category\",\n      \"enum\": [\n        \"Hair Color\",\n \
  \       \"Hair Care\",\n        \"Nail\",\n        \"Skin Care\",\n        \"Tools & Appliances\",\n        \"Salon Furniture\",\n        \"Salon Supplies\",\n        \"Accessories\"\n      ]\n    },\n    \"subcategory\": {\n      \"type\": \"string\",\n      \"description\": \"Product subcategory\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Retail price in USD\"\n    },\n    \"professional_price\": {\n      \"type\": \"number\",\n      \"description\": \"Professional (BSG) price for licensed salon professionals\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\",\n      \"description\": \"Currency code\"\n    },\n    \"upc\": {\n      \"type\": \"string\",\n      \"description\": \"Universal Product Code\"\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"url\": {\n            \"type\": \"string\",\n            \"format\"\
  : \"uri\"\n          },\n          \"alt\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"primary\", \"alternate\", \"swatch\"]\n          }\n        }\n      },\n      \"description\": \"Product image URLs\"\n    },\n    \"available_online\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether product is available for online purchase\"\n    },\n    \"available_in_store\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether product is available in physical stores\"\n    },\n    \"professional_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether product is restricted to licensed professionals (BSG only)\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"Sales channel\",\n      \"enum\": [\"sally\", \"bsg\", \"both\"]\n    },\n    \"ratings\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"average\"\
  : {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 5\n        },\n        \"count\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\", \"brand\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sally-beauty-holdings/refs/heads/main/json-schema/sally-beauty-product-schema.json
tags:
- Beauty
- Retail
- Ecommerce
- Professional
- Consumer
title: Sally Beauty Product
---

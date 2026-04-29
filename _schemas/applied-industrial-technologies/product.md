---
description: An industrial product distributed by Applied Industrial Technologies
layout: schema
name: Product
properties_list:
- description: Unique product identifier
  name: productId
  type: string
- description: Manufacturer part number
  name: partNumber
  type: string
- description: Product name
  name: name
  type: string
- description: Product description
  name: description
  type: string
- description: Product category (bearings, power transmission, etc.)
  name: category
  type: string
- description: Product manufacturer
  name: manufacturer
  type: string
- description: Unit price in USD
  name: price
  type: number
- description: Whether the product is in stock
  name: inStock
  type: boolean
- description: Lead time in days if not in stock
  name: leadTimeDays
  type: integer
provider_name: Applied Industrial Technologies
provider_slug: applied-industrial-technologies
schema_file: json-schema/product-schema.json
slug: product
source_filename: product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/applied-industrial-technologies/main/json-schema/product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"An industrial product distributed by Applied Industrial Technologies\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier\"\n    },\n    \"partNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer part number\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category (bearings, power transmission, etc.)\"\n    },\n    \"manufacturer\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Product manufacturer\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Unit price in USD\"\n    },\n    \"inStock\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product is in stock\"\n    },\n    \"leadTimeDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Lead time in days if not in stock\"\n    }\n  },\n  \"required\": [\n    \"productId\",\n    \"partNumber\",\n    \"name\",\n    \"category\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/applied-industrial-technologies/refs/heads/main/json-schema/product-schema.json
tags:
- Industrial Distribution
- Bearings
- Power Transmission
- Fluid Power
- Supply Chain
title: Product
---

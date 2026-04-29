---
description: An automotive part or product.
layout: schema
name: Product
properties_list:
- description: Product SKU.
  name: id
  type: string
- description: Product name.
  name: name
  type: string
- description: Manufacturer part number.
  name: partNumber
  type: string
- description: Brand name.
  name: brand
  type: string
- description: Product description.
  name: description
  type: string
- description: Current retail price.
  name: price
  type: number
- description: Whether available.
  name: available
  type: boolean
- description: Product category identifier.
  name: categoryId
  type: string
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-product-schema.json
slug: catalog-api-product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Product\",\n  \"description\": \"An automotive part or product.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Product SKU.\",\n      \"example\": \"SKU-123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name.\",\n      \"example\": \"Duralast Gold Brake Pad Set\"\n    },\n    \"partNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer part number.\",\n      \"example\": \"MKD1083\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Brand name.\",\n      \"example\": \"Duralast Gold\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Current retail price.\",\n      \"example\": 54.99\n\
  \    },\n    \"available\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether available.\",\n      \"example\": true\n    },\n    \"categoryId\": {\n      \"type\": \"string\",\n      \"description\": \"Product category identifier.\",\n      \"example\": \"brake-pads\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-product-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: Product
---

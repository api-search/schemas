---
description: A product is something that can be sold by the gift shop, such as t-shirts, hoodies, and other pb33f branded merchandise.
layout: schema
name: pb33f Giftshop Product
properties_list:
- description: The unique identifier for the product.
  name: id
  type: string
- description: A short code for the product, easily human readable.
  name: shortCode
  type: string
- description: The name of the product.
  name: name
  type: string
- description: A description of the product.
  name: description
  type: string
- description: The price of the product, as a floating point number.
  name: price
  type: number
- description: The category of the product.
  name: category
  type: string
- description: The URL of the product image.
  name: image
  type: string
provider_name: Princess Beef Heavy Industries
provider_slug: princess-beef-heavy-industries
schema_file: json-schema/product.json
slug: product
source_filename: product.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/princess-beef-heavy-industries/blob/main/json-schema/product.json\",\n  \"title\": \"pb33f Giftshop Product\",\n  \"description\": \"A product is something that can be sold by the gift shop, such as t-shirts, hoodies, and other pb33f branded merchandise.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"shortCode\",\n    \"name\",\n    \"description\",\n    \"price\",\n    \"category\",\n    \"image\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the product.\"\n    },\n    \"shortCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"A short code for the product, easily human readable.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\"\
  : \"The name of the product.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"maxLength\": 500,\n      \"description\": \"A description of the product.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"The price of the product, as a floating point number.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"The category of the product.\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The URL of the product image.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/princess-beef-heavy-industries/refs/heads/main/json-schema/product.json
tags:
- Commerce
- Documentation
- Editors
- Governance
- Platform
- Products
- Rules
title: pb33f Giftshop Product
---

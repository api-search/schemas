---
description: Product schema from Aramark Marko API
layout: schema
name: Product
properties_list:
- description: Product identifier
  name: id
  type: string
- description: Product name
  name: name
  type: string
- description: Product category
  name: category
  type: string
- description: Product price in USD
  name: price
  type: number
- description: Caloric content
  name: calories
  type: integer
- description: List of allergens
  name: allergens
  type: array
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-product-schema.json
slug: marko-api-product
source_filename: marko-api-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Product identifier\",\n      \"example\": \"PROD-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name\",\n      \"example\": \"Grilled Chicken\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category\",\n      \"enum\": [\n        \"ENTREE\",\n        \"SIDE\",\n        \"BEVERAGE\",\n        \"DESSERT\",\n        \"SNACK\"\n      ],\n      \"example\": \"ENTREE\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Product price in USD\",\n      \"example\": 8.95\n    },\n    \"calories\": {\n      \"type\": \"integer\",\n      \"description\": \"Caloric content\",\n      \"example\": 380\n    },\n    \"allergens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of allergens\"\
  ,\n      \"example\": [\n        \"GLUTEN\",\n        \"DAIRY\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"Product schema from Aramark Marko API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-product-schema.json
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: Product
---

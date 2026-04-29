---
description: ''
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
- description: Food and beverage application areas
  name: applications
  type: array
- description: Protein content percentage
  name: protein
  type: number
- description: Product description
  name: description
  type: string
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
schema_file: json-schema/archer-daniels-midland-commodity-data-api-product-schema.json
slug: archer-daniels-midland-commodity-data-api-product
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Product identifier\",\n      \"example\": \"SOY-PROTEIN-CONC-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name\",\n      \"example\": \"Soy Protein Concentrate\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category\",\n      \"enum\": [\n        \"starches\",\n        \"proteins\",\n        \"oils\",\n        \"sweeteners\",\n        \"fibers\",\n        \"flavors\"\n      ],\n      \"example\": \"proteins\"\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Food and beverage application areas\",\n      \"example\": [\n        \"meat-analogs\",\n        \"dairy-alternatives\"\n      ]\n    },\n    \"protein\": {\n      \"type\": \"number\",\n      \"description\": \"Protein\
  \ content percentage\",\n      \"example\": 70.0\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description\",\n      \"example\": \"High-quality soy protein concentrate for food applications\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-product-schema.json\",\n  \"title\": \"Product\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-product-schema.json
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
title: Product
---

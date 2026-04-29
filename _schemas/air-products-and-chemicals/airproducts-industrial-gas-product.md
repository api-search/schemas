---
description: An industrial gas product offered by Air Products
layout: schema
name: IndustrialGasProduct
properties_list:
- description: Unique product identifier
  name: product_id
  type: string
- description: Product name
  name: name
  type: string
- description: Chemical formula
  name: chemical_formula
  type: string
- description: Purity grade classification
  name: purity_grade
  type: string
- description: Purity percentage
  name: purity_percent
  type: number
- description: 'Physical form: gas, liquid, dissolved'
  name: form
  type: string
- description: Industries and applications served
  name: applications
  type: array
- description: DOT hazard class
  name: safety_class
  type: string
provider_name: Air Products and Chemicals
provider_slug: air-products-and-chemicals
schema_file: json-schema/airproducts-industrial-gas-product-schema.json
slug: airproducts-industrial-gas-product
source_filename: airproducts-industrial-gas-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-products-and-chemicals/refs/heads/main/json-schema/airproducts-industrial-gas-product-schema.json\",\n  \"title\": \"IndustrialGasProduct\",\n  \"description\": \"An industrial gas product offered by Air Products\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"product_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product identifier\",\n      \"example\": \"H2-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name\",\n      \"example\": \"Hydrogen (H2)\"\n    },\n    \"chemical_formula\": {\n      \"type\": \"string\",\n      \"description\": \"Chemical formula\",\n      \"example\": \"H2\"\n    },\n    \"purity_grade\": {\n      \"type\": \"string\",\n      \"description\": \"Purity grade classification\",\n      \"example\": \"Ultra High Purity (UHP)\"\n    },\n   \
  \ \"purity_percent\": {\n      \"type\": \"number\",\n      \"description\": \"Purity percentage\",\n      \"example\": 99.999\n    },\n    \"form\": {\n      \"type\": \"string\",\n      \"description\": \"Physical form: gas, liquid, dissolved\",\n      \"example\": \"compressed gas\"\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"description\": \"Industries and applications served\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"safety_class\": {\n      \"type\": \"string\",\n      \"description\": \"DOT hazard class\",\n      \"example\": \"2.1 Flammable Gas\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-products-and-chemicals/refs/heads/main/json-schema/airproducts-industrial-gas-product-schema.json
tags:
- Industrial Gases
- Chemicals
- Energy
- Manufacturing
- Hydrogen
- Enterprise
title: IndustrialGasProduct
---

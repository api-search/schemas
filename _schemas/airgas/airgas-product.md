---
description: An Airgas product including gases, welding equipment, and safety supplies.
layout: schema
name: Product
properties_list:
- description: Airgas product number / SKU.
  name: product_number
  type: string
- description: Product name.
  name: name
  type: string
- description: Product description.
  name: description
  type: string
- description: Product category.
  name: category
  type: string
- description: Type of gas (for gas products).
  name: gas_type
  type: string
- description: Gas purity grade.
  name: grade
  type: string
- description: Cylinder size designation.
  name: cylinder_size
  type: string
- description: Unit of measure for ordering.
  name: unit_of_measure
  type: string
- description: List price per unit.
  name: price
  type: number
- description: Whether the product is available for order.
  name: available
  type: boolean
provider_name: Airgas
provider_slug: airgas
schema_file: json-schema/airgas-product-schema.json
slug: airgas-product
source_filename: airgas-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airgas/refs/heads/main/json-schema/airgas-product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"An Airgas product including gases, welding equipment, and safety supplies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"product_number\": {\n      \"type\": \"string\",\n      \"description\": \"Airgas product number / SKU.\",\n      \"example\": \"OXUS300\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name.\",\n      \"example\": \"Oxygen, Industrial Grade, 300 CF\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description.\",\n      \"example\": \"Industrial grade oxygen in a 300 cubic foot cylinder.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"enum\": [\"gas\", \"welding\", \"safety\", \"tool\", \"mro\"],\n\
  \      \"description\": \"Product category.\",\n      \"example\": \"gas\"\n    },\n    \"gas_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of gas (for gas products).\",\n      \"example\": \"Oxygen\"\n    },\n    \"grade\": {\n      \"type\": \"string\",\n      \"enum\": [\"industrial\", \"medical\", \"food\", \"specialty\", \"research\"],\n      \"description\": \"Gas purity grade.\",\n      \"example\": \"industrial\"\n    },\n    \"cylinder_size\": {\n      \"type\": \"string\",\n      \"description\": \"Cylinder size designation.\",\n      \"example\": \"T-300\"\n    },\n    \"unit_of_measure\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure for ordering.\",\n      \"example\": \"Each\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"List price per unit.\",\n      \"example\": 125.99\n    },\n    \"available\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product is available\
  \ for order.\",\n      \"example\": true\n    }\n  },\n  \"required\": [\"product_number\", \"name\", \"category\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airgas/refs/heads/main/json-schema/airgas-product-schema.json
tags:
- Industrial Gases
- Welding
- Safety
- B2B
- Supply Chain
- Manufacturing
- Healthcare
title: Product
---

---
description: TerminalProduct schema from Adyen API
layout: schema
name: TerminalProduct
properties_list:
- description: Information about items included and integration options.
  name: description
  type: string
- description: The unique identifier of the product.
  name: id
  type: string
- description: A list of parts included in the terminal package.
  name: itemsIncluded
  type: array
- description: The descriptive name of the product.
  name: name
  type: string
- description: The price of the product.
  name: price
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-product-schema.json
slug: management-terminal-product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-product-schema.json\",\n  \"title\": \"TerminalProduct\",\n  \"description\": \"TerminalProduct schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Information about items included and integration options.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the product.\",\n      \"type\": \"string\"\n    },\n    \"itemsIncluded\": {\n      \"description\": \"A list of parts included in the terminal package.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"name\": {\n      \"description\": \"The descriptive name of the product.\",\n      \"type\": \"string\"\n    },\n    \"price\": {\n      \"description\": \"The price\
  \ of the product.\",\n      \"$ref\": \"#/components/schemas/TerminalProductPrice\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-product-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalProduct
---

---
description: TerminalProductPrice schema from Adyen API
layout: schema
name: TerminalProductPrice
properties_list:
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).
  name: currency
  type: string
- description: The price of the item.
  name: value
  type: number
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-product-price-schema.json
slug: management-terminal-product-price
source_filename: management-terminal-product-price-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-product-price-schema.json\",\n  \"title\": \"TerminalProductPrice\",\n  \"description\": \"TerminalProductPrice schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The price of the item.\",\n      \"format\": \"double\",\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-product-price-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalProductPrice
---

---
description: Product that is payable by the payment card. Product codes that are payable by the payment card.
layout: schema
name: AllowedProduct
properties_list:
- description: Product code of item purchased with the transaction.
  name: ProductCode
  type: integer
- description: Standard product code of item purchased with the transaction.
  name: EanUpc
  type: integer
- description: Product name of an item purchased with the transaction.
  name: ProductLabel
  type: string
- description: Additionl information related to the line item.
  name: AdditionalProductInfo
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-allowed-product-schema.json
slug: terminal-allowed-product
source_filename: terminal-allowed-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-allowed-product-schema.json\",\n  \"title\": \"AllowedProduct\",\n  \"description\": \"Product that is payable by the payment card. Product codes that are payable by the payment card.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProductCode\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 20,\n      \"description\": \"Product code of item purchased with the transaction.\"\n    },\n    \"EanUpc\": {\n      \"type\": \"integer\",\n      \"description\": \"Standard product code of item purchased with the transaction.\"\n    },\n    \"ProductLabel\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Product name of an item purchased with the transaction.\"\n    },\n    \"AdditionalProductInfo\": {\n      \"type\": \"string\",\n   \
  \   \"pattern\": \"^.+$\",\n      \"description\": \"Additionl information related to the line item.\"\n    }\n  },\n  \"required\": [\n    \"ProductCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-allowed-product-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AllowedProduct
---

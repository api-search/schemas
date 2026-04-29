---
description: LineItem schema from Adyen API
layout: schema
name: LineItem
properties_list:
- description: Item amount excluding the tax, in minor units.
  name: amountExcludingTax
  type: integer
- description: Item amount including the tax, in minor units.
  name: amountIncludingTax
  type: integer
- description: Brand of the item.
  name: brand
  type: string
- description: Color of the item.
  name: color
  type: string
- description: Description of the line item.
  name: description
  type: string
- description: ID of the line item.
  name: id
  type: string
- description: Link to the picture of the purchased item.
  name: imageUrl
  type: string
- description: Item category, used by the payment methods PayPal and Ratepay.
  name: itemCategory
  type: string
- description: Manufacturer of the item.
  name: manufacturer
  type: string
- description: Link to the purchased item.
  name: productUrl
  type: string
- description: Number of items.
  name: quantity
  type: integer
- description: Email associated with the given product in the basket (usually in electronic gift cards).
  name: receiverEmail
  type: string
- description: Size of the item.
  name: size
  type: string
- description: Stock keeping unit.
  name: sku
  type: string
- description: Tax amount, in minor units.
  name: taxAmount
  type: integer
- description: Tax percentage, in minor units.
  name: taxPercentage
  type: integer
- description: Universal Product Code.
  name: upc
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-line-item-schema.json
slug: checkout-line-item
source_filename: checkout-line-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-line-item-schema.json\",\n  \"title\": \"LineItem\",\n  \"description\": \"LineItem schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amountExcludingTax\": {\n      \"description\": \"Item amount excluding the tax, in minor units.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"amountIncludingTax\": {\n      \"description\": \"Item amount including the tax, in minor units.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"brand\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Brand of the item.\",\n      \"type\": \"string\"\n    },\n    \"color\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Color of the item.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"\
  description\": \"Description of the line item.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"ID of the line item.\",\n      \"type\": \"string\"\n    },\n    \"imageUrl\": {\n      \"description\": \"Link to the picture of the purchased item.\",\n      \"type\": \"string\"\n    },\n    \"itemCategory\": {\n      \"description\": \"Item category, used by the payment methods PayPal and Ratepay.\",\n      \"type\": \"string\"\n    },\n    \"manufacturer\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Manufacturer of the item.\",\n      \"type\": \"string\"\n    },\n    \"productUrl\": {\n      \"description\": \"Link to the purchased item.\",\n      \"type\": \"string\"\n    },\n    \"quantity\": {\n      \"description\": \"Number of items.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"receiverEmail\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Email associated with the given product\
  \ in the basket (usually in electronic gift cards).\",\n      \"type\": \"string\"\n    },\n    \"size\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Size of the item.\",\n      \"type\": \"string\"\n    },\n    \"sku\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Stock keeping unit.\",\n      \"type\": \"string\"\n    },\n    \"taxAmount\": {\n      \"description\": \"Tax amount, in minor units.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"taxPercentage\": {\n      \"description\": \"Tax percentage, in minor units.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"upc\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Universal Product Code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-line-item-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LineItem
---

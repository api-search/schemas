---
description: Represents a single line item in the checkout, including product details and pricing.
layout: schema
name: ItemObject
properties_list:
- description: Customer-facing product name.
  name: display_name
  type: string
- description: Merchant's stock keeping unit identifier for the product.
  name: sku
  type: string
- description: Unit price of the item in cents.
  name: unit_price
  type: integer
- description: Quantity of this item in the order.
  name: qty
  type: integer
- description: URL of the product image.
  name: item_image_url
  type: string
- description: URL of the product page on the merchant's website.
  name: item_url
  type: string
- description: Nested array of category strings representing the product taxonomy.
  name: categories
  type: array
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/checkout-item-object-schema.json
slug: checkout-item-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-item-object-schema.json\",\n  \"title\": \"ItemObject\",\n  \"description\": \"Represents a single line item in the checkout, including product details and pricing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Customer-facing product name.\",\n      \"example\": \"Example Merchant\"\n    },\n    \"sku\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant's stock keeping unit identifier for the product.\",\n      \"example\": \"example_value\"\n    },\n    \"unit_price\": {\n      \"type\": \"integer\",\n      \"description\": \"Unit price of the item in cents.\",\n      \"minimum\": 0,\n      \"example\": 1\n    },\n    \"qty\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity of this item\
  \ in the order.\",\n      \"minimum\": 1,\n      \"example\": 1\n    },\n    \"item_image_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the product image.\",\n      \"example\": \"https://example.com/path\"\n    },\n    \"item_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the product page on the merchant's website.\",\n      \"example\": \"https://example.com/path\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"Nested array of category strings representing the product taxonomy.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"example\": [\n        [\n          \"example_value\"\n        ]\n      ]\n    }\n  },\n  \"required\": [\n    \"display_name\",\n    \"sku\",\n    \"unit_price\",\n    \"qty\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-item-object-schema.json
tags: []
title: ItemObject
---

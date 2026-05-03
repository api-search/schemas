---
description: An inventory item represents the physical goods for a product variant. Inventory items track quantities across locations and contain cost and customs information. Each product variant has a one-to-one relationship with an inventory item.
layout: schema
name: Shopify Inventory Item
properties_list:
- description: Unique numeric identifier for the inventory item
  name: id
  type: integer
- description: The stock keeping unit
  name: sku
  type:
  - string
  - 'null'
- description: The unit cost of the inventory item as a decimal string
  name: cost
  type:
  - string
  - 'null'
- description: Whether Shopify tracks inventory quantities for this item
  name: tracked
  type: boolean
- description: Whether the item requires shipping
  name: requires_shipping
  type: boolean
- description: The two-letter ISO 3166-1 country code where the item was manufactured
  name: country_code_of_origin
  type:
  - string
  - 'null'
- description: The province or state code where the item was manufactured
  name: province_code_of_origin
  type:
  - string
  - 'null'
- description: The Harmonized System code for customs classification
  name: harmonized_system_code
  type:
  - string
  - 'null'
- description: Country-specific HS codes for customs
  name: country_harmonized_system_codes
  type: array
- description: When the inventory item was created
  name: created_at
  type: string
- description: When the inventory item was last updated
  name: updated_at
  type: string
- description: The GraphQL Admin API identifier
  name: admin_graphql_api_id
  type: string
provider_name: Shopify
provider_slug: shopify
schema_file: json-schema/shopify-inventory-item-schema.json
slug: shopify-inventory-item
source_filename: shopify-inventory-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://shopify.dev/schemas/inventory-item.json\",\n  \"title\": \"Shopify Inventory Item\",\n  \"description\": \"An inventory item represents the physical goods for a product variant. Inventory items track quantities across locations and contain cost and customs information. Each product variant has a one-to-one relationship with an inventory item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the inventory item\"\n    },\n    \"sku\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The stock keeping unit\"\n    },\n    \"cost\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The unit cost of the inventory item as a decimal string\"\n    },\n    \"tracked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Shopify tracks inventory\
  \ quantities for this item\"\n    },\n    \"requires_shipping\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the item requires shipping\"\n    },\n    \"country_code_of_origin\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The two-letter ISO 3166-1 country code where the item was manufactured\"\n    },\n    \"province_code_of_origin\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The province or state code where the item was manufactured\"\n    },\n    \"harmonized_system_code\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The Harmonized System code for customs classification\"\n    },\n    \"country_harmonized_system_codes\": {\n      \"type\": \"array\",\n      \"description\": \"Country-specific HS codes for customs\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"harmonized_system_code\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The country-specific HS code\"\n          },\n          \"country_code\": {\n            \"type\": \"string\",\n            \"description\": \"The two-letter ISO country code\"\n          }\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the inventory item was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the inventory item was last updated\"\n    },\n    \"admin_graphql_api_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL Admin API identifier\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/json-schema/shopify-inventory-item-schema.json
tags:
- Commerce
- Ecommerce
- Payments
- Retail
- Shopping Cart
- T1
title: Shopify Inventory Item
---

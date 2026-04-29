---
description: Inventory availability result for a product across stores.
layout: schema
name: InventoryResult
properties_list:
- description: Product SKU.
  name: productId
  type: string
- description: Store inventory records.
  name: stores
  type: array
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-inventoryresult-schema.json
slug: catalog-api-inventoryresult
source_filename: catalog-api-inventoryresult-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventoryResult\",\n  \"description\": \"Inventory availability result for a product across stores.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Product SKU.\",\n      \"example\": \"SKU-123456\"\n    },\n    \"stores\": {\n      \"type\": \"array\",\n      \"description\": \"Store inventory records.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/StoreInventory\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-inventoryresult-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: InventoryResult
---

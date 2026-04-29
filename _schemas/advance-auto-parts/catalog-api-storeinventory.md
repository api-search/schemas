---
description: Inventory at a specific store.
layout: schema
name: StoreInventory
properties_list:
- description: Store identifier.
  name: storeId
  type: string
- description: Store name.
  name: storeName
  type: string
- description: Available quantity.
  name: quantity
  type: integer
- description: Whether in stock.
  name: available
  type: boolean
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/catalog-api-storeinventory-schema.json
slug: catalog-api-storeinventory
source_filename: catalog-api-storeinventory-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StoreInventory\",\n  \"description\": \"Inventory at a specific store.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"storeId\": {\n      \"type\": \"string\",\n      \"description\": \"Store identifier.\",\n      \"example\": \"store-001\"\n    },\n    \"storeName\": {\n      \"type\": \"string\",\n      \"description\": \"Store name.\",\n      \"example\": \"Advance Auto Parts - Main St\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Available quantity.\",\n      \"example\": 4\n    },\n    \"available\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether in stock.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/catalog-api-storeinventory-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: StoreInventory
---

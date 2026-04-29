---
description: Inventory availability record for a product
layout: schema
name: InventoryItem
properties_list:
- description: Acuity Brands product number
  name: productNumber
  type: string
- description: Product description
  name: description
  type: string
- description: Brand name
  name: brand
  type: string
- description: Total available quantity across all warehouses
  name: totalQuantity
  type: integer
- description: Per-warehouse availability
  name: warehouses
  type: array
- description: Last inventory update time
  name: updatedAt
  type: string
provider_name: acuity-brands
provider_slug: acuity-brands
schema_file: json-schema/acuity-brands-inventory-item-schema.json
slug: acuity-brands-inventory-item
source_filename: acuity-brands-inventory-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-inventory-item-schema.json\",\n  \"title\": \"InventoryItem\",\n  \"description\": \"Inventory availability record for a product\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Acuity Brands product number\",\n      \"example\": \"LBL4 48L ADP\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description\",\n      \"example\": \"4FT LED Wrap Light 4800 Lumens\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Brand name\",\n      \"example\": \"Lithonia Lighting\"\n    },\n    \"totalQuantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Total available quantity across all warehouses\",\n      \"example\": 250\n    },\n    \"warehouses\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Per-warehouse availability\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"code\": {\n            \"type\": \"string\",\n            \"example\": \"ATL\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Atlanta Distribution Center\"\n          },\n          \"quantity\": {\n            \"type\": \"integer\",\n            \"example\": 150\n          },\n          \"estimatedShipDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\",\n            \"example\": \"2026-04-22\"\n          }\n        }\n      }\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last inventory update time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-inventory-item-schema.json
tags: []
title: InventoryItem
---

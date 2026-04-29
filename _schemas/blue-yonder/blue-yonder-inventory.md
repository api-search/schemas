---
description: JSON Schema for a Blue Yonder WMS inventory position representing stock at a warehouse location.
layout: schema
name: Blue Yonder Inventory Position
properties_list:
- description: Unique inventory position identifier
  name: positionId
  type: string
- description: Item/SKU identifier
  name: itemId
  type: string
- description: ''
  name: itemDescription
  type: string
- description: Warehouse location identifier (bin, rack, slot)
  name: locationId
  type: string
- description: ''
  name: locationName
  type: string
- description: Warehouse zone (e.g., Receiving, Storage, Shipping)
  name: zone
  type: string
- description: ''
  name: quantityOnHand
  type: number
- description: ''
  name: quantityAvailable
  type: number
- description: ''
  name: quantityReserved
  type: number
- description: Unit of measure (e.g., EA, CS, LB, KG)
  name: unitOfMeasure
  type: string
- description: ''
  name: lotNumber
  type: string
- description: ''
  name: serialNumber
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: lastUpdated
  type: string
provider_name: blue-yonder
provider_slug: blue-yonder
schema_file: json-schema/blue-yonder-inventory-schema.json
slug: blue-yonder-inventory
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/json-schema/blue-yonder-inventory-schema.json\",\n  \"title\": \"Blue Yonder Inventory Position\",\n  \"description\": \"JSON Schema for a Blue Yonder WMS inventory position representing stock at a warehouse location.\",\n  \"type\": \"object\",\n  \"required\": [\"positionId\", \"itemId\", \"locationId\", \"quantityOnHand\"],\n  \"properties\": {\n    \"positionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique inventory position identifier\"\n    },\n    \"itemId\": {\n      \"type\": \"string\",\n      \"description\": \"Item/SKU identifier\"\n    },\n    \"itemDescription\": {\n      \"type\": \"string\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"Warehouse location identifier (bin, rack, slot)\"\n    },\n    \"locationName\": {\n      \"type\": \"string\"\
  \n    },\n    \"zone\": {\n      \"type\": \"string\",\n      \"description\": \"Warehouse zone (e.g., Receiving, Storage, Shipping)\"\n    },\n    \"quantityOnHand\": {\n      \"type\": \"number\",\n      \"minimum\": 0\n    },\n    \"quantityAvailable\": {\n      \"type\": \"number\",\n      \"minimum\": 0\n    },\n    \"quantityReserved\": {\n      \"type\": \"number\",\n      \"minimum\": 0\n    },\n    \"unitOfMeasure\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure (e.g., EA, CS, LB, KG)\"\n    },\n    \"lotNumber\": {\n      \"type\": \"string\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Available\", \"Reserved\", \"Quarantine\", \"Damaged\"]\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/json-schema/blue-yonder-inventory-schema.json
tags: []
title: Blue Yonder Inventory Position
---

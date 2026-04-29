---
description: ''
layout: schema
name: InventoryItem
properties_list:
- description: Inventory item identifier
  name: inventoryItemId
  type: integer
- description: Item number
  name: segment1
  type: string
- description: Item description
  name: description
  type: string
- description: Extended item description
  name: longDescription
  type: string
- description: Primary unit of measure
  name: primaryUomCode
  type: string
- description: Item type
  name: itemType
  type: string
- description: Item status code
  name: inventoryItemStatusCode
  type: string
- description: Inventory organization identifier
  name: organizationId
  type: integer
- description: Weight unit of measure
  name: weightUomCode
  type: string
- description: Unit weight
  name: unitWeight
  type: number
- description: Volume unit of measure
  name: volumeUomCode
  type: string
- description: Unit volume
  name: unitVolume
  type: number
- description: Item list price
  name: listPrice
  type: number
- description: ''
  name: purchasingEnabledFlag
  type: string
- description: ''
  name: customerOrderEnabledFlag
  type: string
- description: ''
  name: internalOrderEnabledFlag
  type: string
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-inventory-item-schema.json
slug: supply-chain-inventory-item
source_filename: supply-chain-inventory-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventoryItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inventoryItemId\": {\n      \"type\": \"integer\",\n      \"description\": \"Inventory item identifier\"\n    },\n    \"segment1\": {\n      \"type\": \"string\",\n      \"description\": \"Item number\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Item description\"\n    },\n    \"longDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Extended item description\"\n    },\n    \"primaryUomCode\": {\n      \"type\": \"string\",\n      \"description\": \"Primary unit of measure\"\n    },\n    \"itemType\": {\n      \"type\": \"string\",\n      \"description\": \"Item type\"\n    },\n    \"inventoryItemStatusCode\": {\n      \"type\": \"string\",\n      \"description\": \"Item status code\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Inventory organization identifier\"\n    },\n    \"weightUomCode\": {\n      \"type\": \"string\",\n      \"description\": \"Weight unit of measure\"\n    },\n    \"unitWeight\": {\n      \"type\": \"number\",\n      \"description\": \"Unit weight\"\n    },\n    \"volumeUomCode\": {\n      \"type\": \"string\",\n      \"description\": \"Volume unit of measure\"\n    },\n    \"unitVolume\": {\n      \"type\": \"number\",\n      \"description\": \"Unit volume\"\n    },\n    \"listPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Item list price\"\n    },\n    \"purchasingEnabledFlag\": {\n      \"type\": \"string\"\n    },\n    \"customerOrderEnabledFlag\": {\n      \"type\": \"string\"\n    },\n    \"internalOrderEnabledFlag\": {\n      \"type\": \"string\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-inventory-item-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: InventoryItem
---

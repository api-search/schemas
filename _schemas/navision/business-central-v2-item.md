---
description: ''
layout: schema
name: Item
properties_list:
- description: ''
  name: '@odata.etag'
  type: string
- description: The unique identifier of the item
  name: id
  type: string
- description: The item number
  name: number
  type: string
- description: The item display name
  name: displayName
  type: string
- description: The item display name 2
  name: displayName2
  type: string
- description: The item type
  name: type
  type: string
- description: The item category ID
  name: itemCategoryId
  type: string
- description: The item category code
  name: itemCategoryCode
  type: string
- description: Whether the item is blocked
  name: blocked
  type: boolean
- description: The Global Trade Item Number
  name: gtin
  type: string
- description: The current inventory quantity
  name: inventory
  type: number
- description: The unit price
  name: unitPrice
  type: number
- description: Whether the price includes tax
  name: priceIncludesTax
  type: boolean
- description: The unit cost
  name: unitCost
  type: number
- description: The tax group ID
  name: taxGroupId
  type: string
- description: The tax group code
  name: taxGroupCode
  type: string
- description: The base unit of measure ID
  name: baseUnitOfMeasureId
  type: string
- description: The base unit of measure code
  name: baseUnitOfMeasureCode
  type: string
- description: ''
  name: generalProductPostingGroupId
  type: string
- description: ''
  name: generalProductPostingGroupCode
  type: string
- description: ''
  name: inventoryPostingGroupId
  type: string
- description: ''
  name: inventoryPostingGroupCode
  type: string
- description: ''
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-item-schema.json
slug: business-central-v2-item
source_filename: business-central-v2-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Item\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the item\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The item number\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The item display name\"\n    },\n    \"displayName2\": {\n      \"type\": \"string\",\n      \"description\": \"The item display name 2\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The item type\"\n    },\n    \"itemCategoryId\": {\n      \"type\": \"string\",\n      \"description\": \"The item category ID\"\n    },\n    \"itemCategoryCode\": {\n      \"type\": \"string\",\n      \"description\": \"The item category code\"\n    },\n    \"blocked\": {\n   \
  \   \"type\": \"boolean\",\n      \"description\": \"Whether the item is blocked\"\n    },\n    \"gtin\": {\n      \"type\": \"string\",\n      \"description\": \"The Global Trade Item Number\"\n    },\n    \"inventory\": {\n      \"type\": \"number\",\n      \"description\": \"The current inventory quantity\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"The unit price\"\n    },\n    \"priceIncludesTax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the price includes tax\"\n    },\n    \"unitCost\": {\n      \"type\": \"number\",\n      \"description\": \"The unit cost\"\n    },\n    \"taxGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"The tax group ID\"\n    },\n    \"taxGroupCode\": {\n      \"type\": \"string\",\n      \"description\": \"The tax group code\"\n    },\n    \"baseUnitOfMeasureId\": {\n      \"type\": \"string\",\n      \"description\": \"The base unit of measure ID\"\n    },\n    \"baseUnitOfMeasureCode\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The base unit of measure code\"\n    },\n    \"generalProductPostingGroupId\": {\n      \"type\": \"string\"\n    },\n    \"generalProductPostingGroupCode\": {\n      \"type\": \"string\"\n    },\n    \"inventoryPostingGroupId\": {\n      \"type\": \"string\"\n    },\n    \"inventoryPostingGroupCode\": {\n      \"type\": \"string\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-item-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Item
---

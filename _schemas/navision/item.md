---
description: Represents an inventory item entity in Dynamics 365 Business Central. Items are the goods or services that the company buys, sells, or holds in inventory. Each item record contains pricing, categorization, unit of measure, tax, and posting group information.
layout: schema
name: Item
properties_list:
- description: ETag for optimistic concurrency control
  name: '@odata.etag'
  type: string
- description: The unique identifier (GUID) of the item record
  name: id
  type: string
- description: The item number, a unique business identifier assigned automatically or manually
  name: number
  type: string
- description: The primary display name or description of the item
  name: displayName
  type: string
- description: A secondary display name or additional description for the item
  name: displayName2
  type: string
- description: 'The type of item: Inventory (physical goods tracked in stock), Service (labor or services), or Non-Inventory (physical goods not tracked in stock)'
  name: type
  type: string
- description: The unique identifier of the item category
  name: itemCategoryId
  type: string
- description: The code of the item category used for grouping and reporting
  name: itemCategoryCode
  type: string
- description: Indicates whether the item is blocked from being used in transactions
  name: blocked
  type: boolean
- description: The Global Trade Item Number (barcode) for the item
  name: gtin
  type: string
- description: The current quantity in inventory (read-only, computed from item ledger entries)
  name: inventory
  type: number
- description: The default selling unit price of the item
  name: unitPrice
  type: number
- description: Indicates whether the unit price includes tax
  name: priceIncludesTax
  type: boolean
- description: The unit cost of the item used for inventory valuation
  name: unitCost
  type: number
- description: The unique identifier of the tax group for the item
  name: taxGroupId
  type: string
- description: The tax group code that determines how the item is taxed
  name: taxGroupCode
  type: string
- description: The unique identifier of the base unit of measure
  name: baseUnitOfMeasureId
  type: string
- description: The base unit of measure code (e.g., PCS, KG, EA)
  name: baseUnitOfMeasureCode
  type: string
- description: The unique identifier of the general product posting group
  name: generalProductPostingGroupId
  type: string
- description: The general product posting group code used for G/L account mapping
  name: generalProductPostingGroupCode
  type: string
- description: The unique identifier of the inventory posting group
  name: inventoryPostingGroupId
  type: string
- description: The inventory posting group code used for inventory valuation posting
  name: inventoryPostingGroupCode
  type: string
- description: The date and time the item record was last modified (read-only)
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/item.json
slug: item
source_filename: item.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://example.com/schemas/navision/item.json\",\n  \"title\": \"Item\",\n  \"description\": \"Represents an inventory item entity in Dynamics 365 Business Central. Items are the goods or services that the company buys, sells, or holds in inventory. Each item record contains pricing, categorization, unit of measure, tax, and posting group information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for optimistic concurrency control\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier (GUID) of the item record\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The item number, a unique business identifier assigned automatically or manually\"\n    },\n    \"displayName\": {\n\
  \      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The primary display name or description of the item\"\n    },\n    \"displayName2\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"A secondary display name or additional description for the item\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"Inventory\", \"Service\", \"Non-Inventory\"],\n      \"description\": \"The type of item: Inventory (physical goods tracked in stock), Service (labor or services), or Non-Inventory (physical goods not tracked in stock)\"\n    },\n    \"itemCategoryId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the item category\"\n    },\n    \"itemCategoryCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The code of the item category used for grouping and reporting\"\n    },\n    \"blocked\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Indicates whether the item is blocked from being used in transactions\"\n    },\n    \"gtin\": {\n      \"type\": \"string\",\n      \"maxLength\": 14,\n      \"description\": \"The Global Trade Item Number (barcode) for the item\"\n    },\n    \"inventory\": {\n      \"type\": \"number\",\n      \"description\": \"The current quantity in inventory (read-only, computed from item ledger entries)\",\n      \"readOnly\": true\n    },\n    \"unitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"The default selling unit price of the item\"\n    },\n    \"priceIncludesTax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the unit price includes tax\"\n    },\n    \"unitCost\": {\n      \"type\": \"number\",\n      \"description\": \"The unit cost of the item used for inventory valuation\"\n    },\n    \"taxGroupId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique\
  \ identifier of the tax group for the item\"\n    },\n    \"taxGroupCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The tax group code that determines how the item is taxed\"\n    },\n    \"baseUnitOfMeasureId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the base unit of measure\"\n    },\n    \"baseUnitOfMeasureCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"The base unit of measure code (e.g., PCS, KG, EA)\"\n    },\n    \"generalProductPostingGroupId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the general product posting group\"\n    },\n    \"generalProductPostingGroupCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The general product posting group code used for G/L account mapping\"\n    },\n    \"inventoryPostingGroupId\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the inventory posting group\"\n    },\n    \"inventoryPostingGroupCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The inventory posting group code used for inventory valuation posting\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the item record was last modified (read-only)\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"id\", \"displayName\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/item.json
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

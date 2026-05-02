---
description: An inventory item in Microsoft Dynamics 365, representing a product or service that can be bought or sold.
layout: schema
name: Item
properties_list:
- description: The unique identifier of the item.
  name: id
  type: string
- description: The item number.
  name: number
  type: string
- description: The display name of the item.
  name: displayName
  type: string
- description: The type of item.
  name: type
  type: string
- description: The category code for the item.
  name: itemCategoryCode
  type: string
- description: Indicates whether the item is blocked.
  name: blocked
  type: boolean
- description: The Global Trade Item Number (barcode).
  name: gtin
  type: string
- description: The unit sales price of the item.
  name: unitPrice
  type: number
- description: The unit cost of the item.
  name: unitCost
  type: number
- description: The current inventory quantity.
  name: inventory
  type: number
- description: The tax group code for the item.
  name: taxGroupCode
  type: string
- description: The base unit of measure code.
  name: baseUnitOfMeasureCode
  type: string
- description: The date and time the record was last modified.
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schema_file: json-schema/item.json
slug: item
source_filename: item.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/item.json\",\n  \"title\": \"Item\",\n  \"description\": \"An inventory item in Microsoft Dynamics 365, representing a product or service that can be bought or sold.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the item.\",\n      \"readOnly\": true\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The item number.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the item.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"Inventory\", \"Service\", \"Non-Inventory\"],\n      \"description\": \"The type of item.\"\n    },\n    \"itemCategoryCode\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The category code for the item.\"\n    },\n    \"blocked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the item is blocked.\"\n    },\n    \"gtin\": {\n      \"type\": \"string\",\n      \"description\": \"The Global Trade Item Number (barcode).\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"The unit sales price of the item.\"\n    },\n    \"unitCost\": {\n      \"type\": \"number\",\n      \"description\": \"The unit cost of the item.\"\n    },\n    \"inventory\": {\n      \"type\": \"number\",\n      \"description\": \"The current inventory quantity.\",\n      \"readOnly\": true\n    },\n    \"taxGroupCode\": {\n      \"type\": \"string\",\n      \"description\": \"The tax group code for the item.\"\n    },\n    \"baseUnitOfMeasureCode\": {\n      \"type\": \"string\",\n      \"description\": \"The base unit of measure code.\"\n    },\n    \"lastModifiedDateTime\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/item.json
tags:
- CRM
- ERP
- Microsoft Dynamics
title: Item
---

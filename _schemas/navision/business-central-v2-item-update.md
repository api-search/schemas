---
description: ''
layout: schema
name: ItemUpdate
properties_list:
- description: ''
  name: displayName
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: itemCategoryCode
  type: string
- description: ''
  name: blocked
  type: boolean
- description: ''
  name: gtin
  type: string
- description: ''
  name: unitPrice
  type: number
- description: ''
  name: unitCost
  type: number
- description: ''
  name: taxGroupCode
  type: string
- description: ''
  name: baseUnitOfMeasureCode
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-item-update-schema.json
slug: business-central-v2-item-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ItemUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"itemCategoryCode\": {\n      \"type\": \"string\"\n    },\n    \"blocked\": {\n      \"type\": \"boolean\"\n    },\n    \"gtin\": {\n      \"type\": \"string\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\"\n    },\n    \"unitCost\": {\n      \"type\": \"number\"\n    },\n    \"taxGroupCode\": {\n      \"type\": \"string\"\n    },\n    \"baseUnitOfMeasureCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-item-update-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: ItemUpdate
---

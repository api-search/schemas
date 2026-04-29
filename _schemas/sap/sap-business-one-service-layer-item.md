---
description: ''
layout: schema
name: Item
properties_list:
- description: Unique item code
  name: ItemCode
  type: string
- description: Item description
  name: ItemName
  type: string
- description: Item type
  name: ItemType
  type: string
- description: Item group code
  name: ItemsGroupCode
  type: integer
- description: Current quantity in stock
  name: QuantityOnStock
  type: number
- description: Average or standard price
  name: AvgStdPrice
  type: number
- description: Default sales unit of measure
  name: SalesUnit
  type: string
- description: Default purchase unit of measure
  name: PurchaseUnit
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-one-service-layer-item-schema.json
slug: sap-business-one-service-layer-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Item\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ItemCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique item code\"\n    },\n    \"ItemName\": {\n      \"type\": \"string\",\n      \"description\": \"Item description\"\n    },\n    \"ItemType\": {\n      \"type\": \"string\",\n      \"description\": \"Item type\"\n    },\n    \"ItemsGroupCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Item group code\"\n    },\n    \"QuantityOnStock\": {\n      \"type\": \"number\",\n      \"description\": \"Current quantity in stock\"\n    },\n    \"AvgStdPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Average or standard price\"\n    },\n    \"SalesUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Default sales unit of measure\"\n    },\n    \"PurchaseUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Default\
  \ purchase unit of measure\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-one-service-layer-item-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: Item
---

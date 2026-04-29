---
description: ''
layout: schema
name: SalesOrderLine
properties_list:
- description: Line identifier
  name: lineId
  type: integer
- description: Line number
  name: lineNumber
  type: integer
- description: Ordered item number
  name: orderedItem
  type: string
- description: Inventory item identifier
  name: inventoryItemId
  type: integer
- description: Ordered quantity
  name: orderedQuantity
  type: number
- description: Unit of measure
  name: orderQuantityUom
  type: string
- description: Unit selling price
  name: unitSellingPrice
  type: number
- description: Unit list price
  name: unitListPrice
  type: number
- description: ''
  name: lineAmount
  type: number
- description: Scheduled ship date
  name: scheduleShipDate
  type: string
- description: Actual ship date
  name: actualShipDate
  type: string
- description: Line flow status
  name: flowStatusCode
  type: string
- description: ''
  name: shippedQuantity
  type: number
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-sales-order-line-schema.json
slug: supply-chain-sales-order-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineId\": {\n      \"type\": \"integer\",\n      \"description\": \"Line identifier\"\n    },\n    \"lineNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Line number\"\n    },\n    \"orderedItem\": {\n      \"type\": \"string\",\n      \"description\": \"Ordered item number\"\n    },\n    \"inventoryItemId\": {\n      \"type\": \"integer\",\n      \"description\": \"Inventory item identifier\"\n    },\n    \"orderedQuantity\": {\n      \"type\": \"number\",\n      \"description\": \"Ordered quantity\"\n    },\n    \"orderQuantityUom\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure\"\n    },\n    \"unitSellingPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Unit selling price\"\n    },\n    \"unitListPrice\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Unit list price\"\n    },\n    \"lineAmount\": {\n      \"type\": \"number\"\n    },\n    \"scheduleShipDate\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduled ship date\"\n    },\n    \"actualShipDate\": {\n      \"type\": \"string\",\n      \"description\": \"Actual ship date\"\n    },\n    \"flowStatusCode\": {\n      \"type\": \"string\",\n      \"description\": \"Line flow status\"\n    },\n    \"shippedQuantity\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-sales-order-line-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: SalesOrderLine
---

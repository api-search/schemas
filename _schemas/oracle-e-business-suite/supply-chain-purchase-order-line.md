---
description: ''
layout: schema
name: PurchaseOrderLine
properties_list:
- description: Purchase order line identifier
  name: poLineId
  type: integer
- description: Line number
  name: lineNum
  type: integer
- description: Line type
  name: lineType
  type: string
- description: Inventory item identifier
  name: itemId
  type: integer
- description: Item description
  name: itemDescription
  type: string
- description: Item category identifier
  name: categoryId
  type: integer
- description: Ordered quantity
  name: quantity
  type: number
- description: Unit of measure
  name: unitMeasLookupCode
  type: string
- description: Unit price
  name: unitPrice
  type: number
- description: Line amount
  name: amount
  type: number
- description: Need-by date
  name: needByDate
  type: string
- description: Promised date
  name: promisedDate
  type: string
- description: Line close status
  name: closedCode
  type: string
- description: ''
  name: shipments
  type: array
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-purchase-order-line-schema.json
slug: supply-chain-purchase-order-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrderLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"poLineId\": {\n      \"type\": \"integer\",\n      \"description\": \"Purchase order line identifier\"\n    },\n    \"lineNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Line number\"\n    },\n    \"lineType\": {\n      \"type\": \"string\",\n      \"description\": \"Line type\"\n    },\n    \"itemId\": {\n      \"type\": \"integer\",\n      \"description\": \"Inventory item identifier\"\n    },\n    \"itemDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Item description\"\n    },\n    \"categoryId\": {\n      \"type\": \"integer\",\n      \"description\": \"Item category identifier\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Ordered quantity\"\n    },\n    \"unitMeasLookupCode\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Unit of measure\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Unit price\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Line amount\"\n    },\n    \"needByDate\": {\n      \"type\": \"string\",\n      \"description\": \"Need-by date\"\n    },\n    \"promisedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Promised date\"\n    },\n    \"closedCode\": {\n      \"type\": \"string\",\n      \"description\": \"Line close status\"\n    },\n    \"shipments\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-purchase-order-line-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: PurchaseOrderLine
---

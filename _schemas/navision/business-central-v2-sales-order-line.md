---
description: ''
layout: schema
name: SalesOrderLine
properties_list:
- description: ''
  name: '@odata.etag'
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: documentId
  type: string
- description: ''
  name: sequence
  type: integer
- description: ''
  name: itemId
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: lineType
  type: string
- description: ''
  name: lineObjectNumber
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: description2
  type: string
- description: ''
  name: unitOfMeasureId
  type: string
- description: ''
  name: unitOfMeasureCode
  type: string
- description: ''
  name: quantity
  type: number
- description: ''
  name: unitPrice
  type: number
- description: ''
  name: discountAmount
  type: number
- description: ''
  name: discountPercent
  type: number
- description: ''
  name: discountAppliedBeforeTax
  type: boolean
- description: ''
  name: amountExcludingTax
  type: number
- description: ''
  name: taxCode
  type: string
- description: ''
  name: taxPercent
  type: number
- description: ''
  name: totalTaxAmount
  type: number
- description: ''
  name: amountIncludingTax
  type: number
- description: ''
  name: netAmount
  type: number
- description: ''
  name: netTaxAmount
  type: number
- description: ''
  name: netAmountIncludingTax
  type: number
- description: ''
  name: shipmentDate
  type: string
- description: ''
  name: shippedQuantity
  type: number
- description: ''
  name: invoicedQuantity
  type: number
- description: ''
  name: invoiceQuantity
  type: number
- description: ''
  name: shipQuantity
  type: number
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-sales-order-line-schema.json
slug: business-central-v2-sales-order-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"documentId\": {\n      \"type\": \"string\"\n    },\n    \"sequence\": {\n      \"type\": \"integer\"\n    },\n    \"itemId\": {\n      \"type\": \"string\"\n    },\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"lineType\": {\n      \"type\": \"string\"\n    },\n    \"lineObjectNumber\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"description2\": {\n      \"type\": \"string\"\n    },\n    \"unitOfMeasureId\": {\n      \"type\": \"string\"\n    },\n    \"unitOfMeasureCode\": {\n      \"type\": \"string\"\n    },\n    \"quantity\": {\n      \"type\": \"number\"\n    },\n    \"unitPrice\": {\n      \"type\": \"number\"\n    },\n    \"discountAmount\"\
  : {\n      \"type\": \"number\"\n    },\n    \"discountPercent\": {\n      \"type\": \"number\"\n    },\n    \"discountAppliedBeforeTax\": {\n      \"type\": \"boolean\"\n    },\n    \"amountExcludingTax\": {\n      \"type\": \"number\"\n    },\n    \"taxCode\": {\n      \"type\": \"string\"\n    },\n    \"taxPercent\": {\n      \"type\": \"number\"\n    },\n    \"totalTaxAmount\": {\n      \"type\": \"number\"\n    },\n    \"amountIncludingTax\": {\n      \"type\": \"number\"\n    },\n    \"netAmount\": {\n      \"type\": \"number\"\n    },\n    \"netTaxAmount\": {\n      \"type\": \"number\"\n    },\n    \"netAmountIncludingTax\": {\n      \"type\": \"number\"\n    },\n    \"shipmentDate\": {\n      \"type\": \"string\"\n    },\n    \"shippedQuantity\": {\n      \"type\": \"number\"\n    },\n    \"invoicedQuantity\": {\n      \"type\": \"number\"\n    },\n    \"invoiceQuantity\": {\n      \"type\": \"number\"\n    },\n    \"shipQuantity\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-sales-order-line-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: SalesOrderLine
---

---
description: ''
layout: schema
name: PurchaseInvoice
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: number
  type: string
- description: ''
  name: invoiceDate
  type: string
- description: ''
  name: postingDate
  type: string
- description: ''
  name: dueDate
  type: string
- description: ''
  name: vendorId
  type: string
- description: ''
  name: vendorNumber
  type: string
- description: ''
  name: vendorName
  type: string
- description: ''
  name: currencyCode
  type: string
- description: ''
  name: pricesIncludeTax
  type: boolean
- description: ''
  name: totalAmountExcludingTax
  type: number
- description: ''
  name: totalTaxAmount
  type: number
- description: ''
  name: totalAmountIncludingTax
  type: number
- description: ''
  name: status
  type: string
- description: ''
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-purchase-invoice-schema.json
slug: business-central-v2-purchase-invoice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseInvoice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"type\": \"string\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\"\n    },\n    \"postingDate\": {\n      \"type\": \"string\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\"\n    },\n    \"vendorId\": {\n      \"type\": \"string\"\n    },\n    \"vendorNumber\": {\n      \"type\": \"string\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    },\n    \"pricesIncludeTax\": {\n      \"type\": \"boolean\"\n    },\n    \"totalAmountExcludingTax\": {\n      \"type\": \"number\"\n    },\n    \"totalTaxAmount\": {\n      \"type\": \"number\"\n    },\n    \"totalAmountIncludingTax\": {\n      \"type\": \"number\"\n    },\n    \"status\": {\n      \"type\": \"string\"\
  \n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-purchase-invoice-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: PurchaseInvoice
---

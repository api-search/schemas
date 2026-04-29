---
description: ''
layout: schema
name: PurchaseOrderCreate
properties_list:
- description: ''
  name: orderDate
  type: string
- description: ''
  name: vendorId
  type: string
- description: ''
  name: vendorNumber
  type: string
- description: ''
  name: currencyCode
  type: string
- description: ''
  name: pricesIncludeTax
  type: boolean
- description: ''
  name: requestedReceiptDate
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-purchase-order-create-schema.json
slug: business-central-v2-purchase-order-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrderCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderDate\": {\n      \"type\": \"string\"\n    },\n    \"vendorId\": {\n      \"type\": \"string\"\n    },\n    \"vendorNumber\": {\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    },\n    \"pricesIncludeTax\": {\n      \"type\": \"boolean\"\n    },\n    \"requestedReceiptDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-purchase-order-create-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: PurchaseOrderCreate
---

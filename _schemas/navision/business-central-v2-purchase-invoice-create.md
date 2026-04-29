---
description: ''
layout: schema
name: PurchaseInvoiceCreate
properties_list:
- description: ''
  name: invoiceDate
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
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-purchase-invoice-create-schema.json
slug: business-central-v2-purchase-invoice-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseInvoiceCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoiceDate\": {\n      \"type\": \"string\"\n    },\n    \"vendorId\": {\n      \"type\": \"string\"\n    },\n    \"vendorNumber\": {\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    },\n    \"pricesIncludeTax\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-purchase-invoice-create-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: PurchaseInvoiceCreate
---

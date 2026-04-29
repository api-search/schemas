---
description: ''
layout: schema
name: PurchaseOrder
properties_list:
- description: ''
  name: '@odata.etag'
  type: string
- description: The unique identifier of the purchase order
  name: id
  type: string
- description: The purchase order number
  name: number
  type: string
- description: The order date
  name: orderDate
  type: string
- description: The posting date
  name: postingDate
  type: string
- description: The vendor ID
  name: vendorId
  type: string
- description: The vendor number
  name: vendorNumber
  type: string
- description: The vendor name
  name: vendorName
  type: string
- description: ''
  name: payToName
  type: string
- description: ''
  name: payToVendorId
  type: string
- description: ''
  name: payToVendorNumber
  type: string
- description: ''
  name: shipToName
  type: string
- description: ''
  name: shipToContact
  type: string
- description: ''
  name: buyFromAddressLine1
  type: string
- description: ''
  name: buyFromAddressLine2
  type: string
- description: ''
  name: buyFromCity
  type: string
- description: ''
  name: buyFromCountry
  type: string
- description: ''
  name: buyFromState
  type: string
- description: ''
  name: buyFromPostCode
  type: string
- description: ''
  name: currencyId
  type: string
- description: ''
  name: currencyCode
  type: string
- description: ''
  name: pricesIncludeTax
  type: boolean
- description: ''
  name: paymentTermsId
  type: string
- description: ''
  name: shipmentMethodId
  type: string
- description: ''
  name: purchaser
  type: string
- description: ''
  name: requestedReceiptDate
  type: string
- description: ''
  name: discountAmount
  type: number
- description: ''
  name: discountAppliedBeforeTax
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
  name: fullyReceived
  type: boolean
- description: ''
  name: status
  type: string
- description: ''
  name: lastModifiedDateTime
  type: string
- description: ''
  name: purchaseOrderLines
  type: array
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-purchase-order-schema.json
slug: business-central-v2-purchase-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PurchaseOrder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the purchase order\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The purchase order number\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"description\": \"The order date\"\n    },\n    \"postingDate\": {\n      \"type\": \"string\",\n      \"description\": \"The posting date\"\n    },\n    \"vendorId\": {\n      \"type\": \"string\",\n      \"description\": \"The vendor ID\"\n    },\n    \"vendorNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The vendor number\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"The vendor name\"\n    },\n    \"payToName\": {\n   \
  \   \"type\": \"string\"\n    },\n    \"payToVendorId\": {\n      \"type\": \"string\"\n    },\n    \"payToVendorNumber\": {\n      \"type\": \"string\"\n    },\n    \"shipToName\": {\n      \"type\": \"string\"\n    },\n    \"shipToContact\": {\n      \"type\": \"string\"\n    },\n    \"buyFromAddressLine1\": {\n      \"type\": \"string\"\n    },\n    \"buyFromAddressLine2\": {\n      \"type\": \"string\"\n    },\n    \"buyFromCity\": {\n      \"type\": \"string\"\n    },\n    \"buyFromCountry\": {\n      \"type\": \"string\"\n    },\n    \"buyFromState\": {\n      \"type\": \"string\"\n    },\n    \"buyFromPostCode\": {\n      \"type\": \"string\"\n    },\n    \"currencyId\": {\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    },\n    \"pricesIncludeTax\": {\n      \"type\": \"boolean\"\n    },\n    \"paymentTermsId\": {\n      \"type\": \"string\"\n    },\n    \"shipmentMethodId\": {\n      \"type\": \"string\"\n    },\n    \"purchaser\":\
  \ {\n      \"type\": \"string\"\n    },\n    \"requestedReceiptDate\": {\n      \"type\": \"string\"\n    },\n    \"discountAmount\": {\n      \"type\": \"number\"\n    },\n    \"discountAppliedBeforeTax\": {\n      \"type\": \"boolean\"\n    },\n    \"totalAmountExcludingTax\": {\n      \"type\": \"number\"\n    },\n    \"totalTaxAmount\": {\n      \"type\": \"number\"\n    },\n    \"totalAmountIncludingTax\": {\n      \"type\": \"number\"\n    },\n    \"fullyReceived\": {\n      \"type\": \"boolean\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\"\n    },\n    \"purchaseOrderLines\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-purchase-order-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: PurchaseOrder
---

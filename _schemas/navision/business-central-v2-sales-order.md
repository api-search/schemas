---
description: ''
layout: schema
name: SalesOrder
properties_list:
- description: ''
  name: '@odata.etag'
  type: string
- description: The unique identifier of the sales order
  name: id
  type: string
- description: The sales order number
  name: number
  type: string
- description: The external document number
  name: externalDocumentNumber
  type: string
- description: The order date
  name: orderDate
  type: string
- description: The posting date
  name: postingDate
  type: string
- description: The customer ID
  name: customerId
  type: string
- description: The customer number
  name: customerNumber
  type: string
- description: The customer name
  name: customerName
  type: string
- description: The bill-to name
  name: billToName
  type: string
- description: The bill-to customer ID
  name: billToCustomerId
  type: string
- description: The bill-to customer number
  name: billToCustomerNumber
  type: string
- description: The ship-to name
  name: shipToName
  type: string
- description: The ship-to contact
  name: shipToContact
  type: string
- description: ''
  name: sellToAddressLine1
  type: string
- description: ''
  name: sellToAddressLine2
  type: string
- description: ''
  name: sellToCity
  type: string
- description: ''
  name: sellToCountry
  type: string
- description: ''
  name: sellToState
  type: string
- description: ''
  name: sellToPostCode
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
  name: salesperson
  type: string
- description: ''
  name: requestedDeliveryDate
  type: string
- description: The total discount amount
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
  name: fullyShipped
  type: boolean
- description: The order status
  name: status
  type: string
- description: ''
  name: lastModifiedDateTime
  type: string
- description: ''
  name: phoneNumber
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: salesOrderLines
  type: array
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-sales-order-schema.json
slug: business-central-v2-sales-order
source_filename: business-central-v2-sales-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the sales order\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The sales order number\"\n    },\n    \"externalDocumentNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The external document number\"\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"description\": \"The order date\"\n    },\n    \"postingDate\": {\n      \"type\": \"string\",\n      \"description\": \"The posting date\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"The customer ID\"\n    },\n    \"customerNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The customer number\"\n    },\n \
  \   \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"The customer name\"\n    },\n    \"billToName\": {\n      \"type\": \"string\",\n      \"description\": \"The bill-to name\"\n    },\n    \"billToCustomerId\": {\n      \"type\": \"string\",\n      \"description\": \"The bill-to customer ID\"\n    },\n    \"billToCustomerNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The bill-to customer number\"\n    },\n    \"shipToName\": {\n      \"type\": \"string\",\n      \"description\": \"The ship-to name\"\n    },\n    \"shipToContact\": {\n      \"type\": \"string\",\n      \"description\": \"The ship-to contact\"\n    },\n    \"sellToAddressLine1\": {\n      \"type\": \"string\"\n    },\n    \"sellToAddressLine2\": {\n      \"type\": \"string\"\n    },\n    \"sellToCity\": {\n      \"type\": \"string\"\n    },\n    \"sellToCountry\": {\n      \"type\": \"string\"\n    },\n    \"sellToState\": {\n      \"type\": \"string\"\n    },\n    \"sellToPostCode\"\
  : {\n      \"type\": \"string\"\n    },\n    \"currencyId\": {\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    },\n    \"pricesIncludeTax\": {\n      \"type\": \"boolean\"\n    },\n    \"paymentTermsId\": {\n      \"type\": \"string\"\n    },\n    \"shipmentMethodId\": {\n      \"type\": \"string\"\n    },\n    \"salesperson\": {\n      \"type\": \"string\"\n    },\n    \"requestedDeliveryDate\": {\n      \"type\": \"string\"\n    },\n    \"discountAmount\": {\n      \"type\": \"number\",\n      \"description\": \"The total discount amount\"\n    },\n    \"discountAppliedBeforeTax\": {\n      \"type\": \"boolean\"\n    },\n    \"totalAmountExcludingTax\": {\n      \"type\": \"number\"\n    },\n    \"totalTaxAmount\": {\n      \"type\": \"number\"\n    },\n    \"totalAmountIncludingTax\": {\n      \"type\": \"number\"\n    },\n    \"fullyShipped\": {\n      \"type\": \"boolean\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"The order status\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"salesOrderLines\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-sales-order-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: SalesOrder
---

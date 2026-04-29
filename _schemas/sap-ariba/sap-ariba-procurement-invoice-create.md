---
description: Request body for creating a new invoice
layout: schema
name: InvoiceCreate
properties_list:
- description: Supplier-assigned invoice number
  name: invoiceNumber
  type: string
- description: Invoice issue date
  name: invoiceDate
  type: string
- description: ''
  name: invoiceType
  type: string
- description: Purchase order number
  name: purchaseOrderReference
  type: string
- description: ''
  name: currency
  type: string
- description: ''
  name: lineItems
  type: array
- description: ''
  name: comments
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-invoice-create-schema.json
slug: sap-ariba-procurement-invoice-create
source_filename: sap-ariba-procurement-invoice-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InvoiceCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new invoice\",\n  \"properties\": {\n    \"invoiceNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier-assigned invoice number\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice issue date\"\n    },\n    \"invoiceType\": {\n      \"type\": \"string\"\n    },\n    \"purchaseOrderReference\": {\n      \"type\": \"string\",\n      \"description\": \"Purchase order number\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\"\n    },\n    \"comments\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-invoice-create-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: InvoiceCreate
---

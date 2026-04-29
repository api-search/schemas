---
description: A line item on an invoice
layout: schema
name: InvoiceLineItem
properties_list:
- description: Line item number on the invoice
  name: lineNumber
  type: string
- description: Referenced purchase order number
  name: purchaseOrderReference
  type: string
- description: Referenced purchase order line item number
  name: poLineNumber
  type: string
- description: Item or service description
  name: description
  type: string
- description: Invoiced quantity
  name: quantity
  type: number
- description: Buyer part number
  name: buyerPartNumber
  type: string
- description: Supplier part number
  name: supplierPartNumber
  type: string
- description: Service period start date
  name: serviceStartDate
  type: string
- description: Service period end date
  name: serviceEndDate
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-invoice-line-item-schema.json
slug: sap-ariba-procurement-invoice-line-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InvoiceLineItem\",\n  \"type\": \"object\",\n  \"description\": \"A line item on an invoice\",\n  \"properties\": {\n    \"lineNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Line item number on the invoice\"\n    },\n    \"purchaseOrderReference\": {\n      \"type\": \"string\",\n      \"description\": \"Referenced purchase order number\"\n    },\n    \"poLineNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Referenced purchase order line item number\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Item or service description\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Invoiced quantity\"\n    },\n    \"buyerPartNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Buyer part number\"\n    },\n    \"supplierPartNumber\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Supplier part number\"\n    },\n    \"serviceStartDate\": {\n      \"type\": \"string\",\n      \"description\": \"Service period start date\"\n    },\n    \"serviceEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"Service period end date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-invoice-line-item-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: InvoiceLineItem
---

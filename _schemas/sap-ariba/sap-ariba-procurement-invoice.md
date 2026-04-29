---
description: An invoice document submitted by a supplier for goods or services delivered against a purchase order
layout: schema
name: Invoice
properties_list:
- description: Internal unique invoice identifier
  name: invoiceId
  type: string
- description: Supplier-assigned invoice number
  name: invoiceNumber
  type: string
- description: Date the invoice was issued
  name: invoiceDate
  type: string
- description: Type of invoice document
  name: invoiceType
  type: string
- description: Primary purchase order number this invoice relates to
  name: purchaseOrderReference
  type: string
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Payment due date
  name: dueDate
  type: string
- description: Invoice line items
  name: lineItems
  type: array
- description: Header-level tax summary
  name: taxDetails
  type: array
- description: Invoice comments or notes
  name: comments
  type: string
- description: Date the invoice was approved
  name: approvalDate
  type: string
- description: Date payment was made
  name: paymentDate
  type: string
- description: Payment transaction reference number
  name: paymentReference
  type: string
- description: Timestamp when the invoice was created in the system
  name: createdDate
  type: string
- description: Timestamp of the last modification
  name: lastModifiedDate
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-invoice-schema.json
slug: sap-ariba-procurement-invoice
source_filename: sap-ariba-procurement-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Invoice\",\n  \"type\": \"object\",\n  \"description\": \"An invoice document submitted by a supplier for goods or services delivered against a purchase order\",\n  \"properties\": {\n    \"invoiceId\": {\n      \"type\": \"string\",\n      \"description\": \"Internal unique invoice identifier\"\n    },\n    \"invoiceNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier-assigned invoice number\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the invoice was issued\"\n    },\n    \"invoiceType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of invoice document\"\n    },\n    \"purchaseOrderReference\": {\n      \"type\": \"string\",\n      \"description\": \"Primary purchase order number this invoice relates to\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency\
  \ code\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\",\n      \"description\": \"Payment due date\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"description\": \"Invoice line items\"\n    },\n    \"taxDetails\": {\n      \"type\": \"array\",\n      \"description\": \"Header-level tax summary\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice comments or notes\"\n    },\n    \"approvalDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the invoice was approved\"\n    },\n    \"paymentDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date payment was made\"\n    },\n    \"paymentReference\": {\n      \"type\": \"string\",\n      \"description\": \"Payment transaction reference number\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the invoice was created in the system\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Timestamp of the last modification\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-invoice-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: Invoice
---

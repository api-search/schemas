---
description: A goods receipt or service confirmation recorded against a purchase order
layout: schema
name: Receipt
properties_list:
- description: Unique receipt identifier
  name: receiptId
  type: string
- description: Reference to the purchase order
  name: purchaseOrderId
  type: string
- description: Date goods were received or services confirmed
  name: receiptDate
  type: string
- description: Type of receipt
  name: receiptType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: lineItems
  type: array
- description: ''
  name: createdDate
  type: string
- description: User who created the receipt
  name: createdBy
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-receipt-schema.json
slug: sap-ariba-procurement-receipt
source_filename: sap-ariba-procurement-receipt-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Receipt\",\n  \"type\": \"object\",\n  \"description\": \"A goods receipt or service confirmation recorded against a purchase order\",\n  \"properties\": {\n    \"receiptId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique receipt identifier\"\n    },\n    \"purchaseOrderId\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to the purchase order\"\n    },\n    \"receiptDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date goods were received or services confirmed\"\n    },\n    \"receiptType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of receipt\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the\
  \ receipt\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-receipt-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: Receipt
---

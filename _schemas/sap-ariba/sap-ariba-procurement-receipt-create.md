---
description: Request body for creating a receipt
layout: schema
name: ReceiptCreate
properties_list:
- description: ''
  name: receiptDate
  type: string
- description: ''
  name: receiptType
  type: string
- description: ''
  name: lineItems
  type: array
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-receipt-create-schema.json
slug: sap-ariba-procurement-receipt-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReceiptCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a receipt\",\n  \"properties\": {\n    \"receiptDate\": {\n      \"type\": \"string\"\n    },\n    \"receiptType\": {\n      \"type\": \"string\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-receipt-create-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: ReceiptCreate
---

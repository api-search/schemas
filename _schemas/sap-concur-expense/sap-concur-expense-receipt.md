---
description: Schema for an SAP Concur Receipt Image — a digital receipt or document image attached to an expense entry for audit and compliance purposes.
layout: schema
name: SAP Concur Receipt Image
properties_list:
- description: The unique identifier of the receipt image
  name: ID
  type: string
- description: The expense entry ID this receipt is associated with
  name: EntryID
  type: string
- description: Temporary presigned URL to download the receipt image file
  name: ReceiptImageURL
  type: string
- description: Whether expense policy requires a receipt for the associated entry
  name: IsRequired
  type: boolean
- description: Type of receipt (e.g., physical, e-receipt, digital tax invoice)
  name: ReceiptType
  type: string
- description: ISO 8601 datetime when the receipt image was uploaded
  name: UploadDate
  type: string
- description: MIME type of the receipt image file
  name: FileType
  type: string
- description: Size of the receipt image file in bytes
  name: FileSizeBytes
  type: integer
- description: Full URI for the receipt image resource
  name: URI
  type: string
provider_name: SAP Concur Expense
provider_slug: sap-concur-expense
schema_file: json-schema/sap-concur-expense-receipt-schema.json
slug: sap-concur-expense-receipt
source_filename: sap-concur-expense-receipt-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/sap-concur-expense/json-schema/sap-concur-expense-receipt-schema.json\",\n  \"title\": \"SAP Concur Receipt Image\",\n  \"description\": \"Schema for an SAP Concur Receipt Image — a digital receipt or document image attached to an expense entry for audit and compliance purposes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the receipt image\"\n    },\n    \"EntryID\": {\n      \"type\": \"string\",\n      \"description\": \"The expense entry ID this receipt is associated with\"\n    },\n    \"ReceiptImageURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Temporary presigned URL to download the receipt image file\"\n    },\n    \"IsRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether expense policy requires\
  \ a receipt for the associated entry\"\n    },\n    \"ReceiptType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of receipt (e.g., physical, e-receipt, digital tax invoice)\",\n      \"enum\": [\"physical\", \"e-receipt\", \"digital-tax-invoice\", \"credit-card\", \"other\"]\n    },\n    \"UploadDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 datetime when the receipt image was uploaded\"\n    },\n    \"FileType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the receipt image file\",\n      \"enum\": [\"image/png\", \"image/jpeg\", \"application/pdf\", \"image/tiff\"]\n    },\n    \"FileSizeBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the receipt image file in bytes\"\n    },\n    \"URI\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Full URI for the receipt image resource\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/json-schema/sap-concur-expense-receipt-schema.json
tags:
- Expense Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
- SAP
- Travel
title: SAP Concur Receipt Image
---

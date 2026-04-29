---
description: A line item on an invoice
layout: schema
name: InvoiceLine
properties_list:
- description: The unique identifier for the line item
  name: Id
  type: string
- description: Line number within the transaction
  name: LineNum
  type: integer
- description: Free-form text description of the line item
  name: Description
  type: string
- description: The total amount for the line item
  name: Amount
  type: number
- description: Specifies the type of line detail
  name: DetailType
  type: string
- description: ''
  name: LinkedTxn
  type: array
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-invoice-line-schema.json
slug: quickbooks-accounting-invoice-line
source_filename: quickbooks-accounting-invoice-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InvoiceLine\",\n  \"type\": \"object\",\n  \"description\": \"A line item on an invoice\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the line item\"\n    },\n    \"LineNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Line number within the transaction\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Free-form text description of the line item\"\n    },\n    \"Amount\": {\n      \"type\": \"number\",\n      \"description\": \"The total amount for the line item\"\n    },\n    \"DetailType\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the type of line detail\"\n    },\n    \"LinkedTxn\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-invoice-line-schema.json
tags:
- Accounting
- Custom Fields
- Financial
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Taxes
- Time Tracking
title: InvoiceLine
---

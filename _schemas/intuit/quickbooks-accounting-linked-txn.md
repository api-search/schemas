---
description: A reference to a linked transaction such as an invoice, payment, or credit memo
layout: schema
name: LinkedTxn
properties_list:
- description: Transaction ID of the related transaction
  name: TxnId
  type: string
- description: The type of the linked transaction
  name: TxnType
  type: string
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-linked-txn-schema.json
slug: quickbooks-accounting-linked-txn
source_filename: quickbooks-accounting-linked-txn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LinkedTxn\",\n  \"type\": \"object\",\n  \"description\": \"A reference to a linked transaction such as an invoice, payment, or credit memo\",\n  \"properties\": {\n    \"TxnId\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction ID of the related transaction\"\n    },\n    \"TxnType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the linked transaction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-linked-txn-schema.json
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
title: LinkedTxn
---

---
description: A Payment records a payment received from a customer. Payments can be applied to one or more outstanding invoices, or left as unapplied credit.
layout: schema
name: Payment
properties_list:
- description: Unique identifier for the payment
  name: Id
  type: string
- description: Version number for optimistic locking
  name: SyncToken
  type: string
- description: The date of the payment transaction
  name: TxnDate
  type: string
- description: Total amount of the payment
  name: TotalAmt
  type: number
- description: Reference number for the payment (e.g., check number)
  name: PaymentRefNum
  type: string
- description: Currency exchange rate
  name: ExchangeRate
  type: number
- description: Lines indicating which invoices or credit memos this payment is applied against
  name: Line
  type: array
- description: Private note for internal use
  name: PrivateNote
  type: string
- description: Amount not yet applied to invoices
  name: UnappliedAmt
  type: number
- description: Whether to process the payment through the Intuit payment gateway
  name: ProcessPayment
  type: boolean
- description: Source of the transaction
  name: TxnSource
  type: string
- description: ''
  name: domain
  type: string
- description: ''
  name: sparse
  type: boolean
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-payment-schema.json
slug: quickbooks-accounting-payment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Payment\",\n  \"type\": \"object\",\n  \"description\": \"A Payment records a payment received from a customer. Payments can be applied to one or more outstanding invoices, or left as unapplied credit.\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the payment\"\n    },\n    \"SyncToken\": {\n      \"type\": \"string\",\n      \"description\": \"Version number for optimistic locking\"\n    },\n    \"TxnDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the payment transaction\"\n    },\n    \"TotalAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Total amount of the payment\"\n    },\n    \"PaymentRefNum\": {\n      \"type\": \"string\",\n      \"description\": \"Reference number for the payment (e.g., check number)\"\n    },\n    \"ExchangeRate\": {\n      \"type\": \"number\",\n   \
  \   \"description\": \"Currency exchange rate\"\n    },\n    \"Line\": {\n      \"type\": \"array\",\n      \"description\": \"Lines indicating which invoices or credit memos this payment is applied against\"\n    },\n    \"PrivateNote\": {\n      \"type\": \"string\",\n      \"description\": \"Private note for internal use\"\n    },\n    \"UnappliedAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Amount not yet applied to invoices\"\n    },\n    \"ProcessPayment\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to process the payment through the Intuit payment gateway\"\n    },\n    \"TxnSource\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the transaction\"\n    },\n    \"domain\": {\n      \"type\": \"string\"\n    },\n    \"sparse\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-payment-schema.json
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
title: Payment
---

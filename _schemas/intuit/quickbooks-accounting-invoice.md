---
description: An Invoice represents a sales form where the customer pays for a product or service later. It creates an accounts receivable transaction.
layout: schema
name: Invoice
properties_list:
- description: Unique identifier for the invoice (assigned by QuickBooks)
  name: Id
  type: string
- description: Version number of the entity, used for optimistic locking. Required for updates.
  name: SyncToken
  type: string
- description: Reference number for the transaction. If not provided, QuickBooks auto-generates one.
  name: DocNumber
  type: string
- description: The date of the transaction. Defaults to the current date.
  name: TxnDate
  type: string
- description: Date when the payment of the transaction is due
  name: DueDate
  type: string
- description: A private note that is not displayed to the customer
  name: PrivateNote
  type: string
- description: A note to the customer displayed on the invoice
  name: CustomerMemo
  type: object
- description: Individual line items of the transaction. At least one line is required.
  name: Line
  type: array
- description: Total amount of the transaction including tax
  name: TotalAmt
  type: number
- description: The balance remaining on the invoice. A value of 0 indicates the invoice is fully paid.
  name: Balance
  type: number
- description: Deposit amount applied to the invoice
  name: Deposit
  type: number
- description: Currency exchange rate (multicurrency enabled companies)
  name: ExchangeRate
  type: number
- description: Date for delivery of goods or services
  name: ShipDate
  type: string
- description: Shipping tracking number
  name: TrackingNum
  type: string
- description: Whether to apply tax after discount
  name: ApplyTaxAfterDiscount
  type: boolean
- description: Printing status of the invoice
  name: PrintStatus
  type: string
- description: Email delivery status of the invoice
  name: EmailStatus
  type: string
- description: Method in which tax is applied
  name: GlobalTaxCalculation
  type: string
- description: Whether online payment is allowed
  name: AllowOnlinePayment
  type: boolean
- description: Whether online credit card payment is allowed
  name: AllowOnlineCreditCardPayment
  type: boolean
- description: Whether online ACH (bank) payment is allowed
  name: AllowOnlineACHPayment
  type: boolean
- description: ''
  name: CustomField
  type: array
- description: ''
  name: LinkedTxn
  type: array
- description: Domain (e.g., QBO)
  name: domain
  type: string
- description: Whether this is a sparse (partial) representation
  name: sparse
  type: boolean
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-invoice-schema.json
slug: quickbooks-accounting-invoice
source_filename: quickbooks-accounting-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Invoice\",\n  \"type\": \"object\",\n  \"description\": \"An Invoice represents a sales form where the customer pays for a product or service later. It creates an accounts receivable transaction.\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the invoice (assigned by QuickBooks)\"\n    },\n    \"SyncToken\": {\n      \"type\": \"string\",\n      \"description\": \"Version number of the entity, used for optimistic locking. Required for updates.\"\n    },\n    \"DocNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Reference number for the transaction. If not provided, QuickBooks auto-generates one.\"\n    },\n    \"TxnDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the transaction. Defaults to the current date.\"\n    },\n    \"DueDate\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Date when the payment of the transaction is due\"\n    },\n    \"PrivateNote\": {\n      \"type\": \"string\",\n      \"description\": \"A private note that is not displayed to the customer\"\n    },\n    \"CustomerMemo\": {\n      \"type\": \"object\",\n      \"description\": \"A note to the customer displayed on the invoice\"\n    },\n    \"Line\": {\n      \"type\": \"array\",\n      \"description\": \"Individual line items of the transaction. At least one line is required.\"\n    },\n    \"TotalAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Total amount of the transaction including tax\"\n    },\n    \"Balance\": {\n      \"type\": \"number\",\n      \"description\": \"The balance remaining on the invoice. A value of 0 indicates the invoice is fully paid.\"\n    },\n    \"Deposit\": {\n      \"type\": \"number\",\n      \"description\": \"Deposit amount applied to the invoice\"\n    },\n    \"ExchangeRate\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Currency exchange rate (multicurrency enabled companies)\"\n    },\n    \"ShipDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date for delivery of goods or services\"\n    },\n    \"TrackingNum\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping tracking number\"\n    },\n    \"ApplyTaxAfterDiscount\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to apply tax after discount\"\n    },\n    \"PrintStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Printing status of the invoice\"\n    },\n    \"EmailStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Email delivery status of the invoice\"\n    },\n    \"GlobalTaxCalculation\": {\n      \"type\": \"string\",\n      \"description\": \"Method in which tax is applied\"\n    },\n    \"AllowOnlinePayment\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether online payment is allowed\"\n    },\n    \"AllowOnlineCreditCardPayment\": {\n     \
  \ \"type\": \"boolean\",\n      \"description\": \"Whether online credit card payment is allowed\"\n    },\n    \"AllowOnlineACHPayment\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether online ACH (bank) payment is allowed\"\n    },\n    \"CustomField\": {\n      \"type\": \"array\"\n    },\n    \"LinkedTxn\": {\n      \"type\": \"array\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Domain (e.g., QBO)\"\n    },\n    \"sparse\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a sparse (partial) representation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-invoice-schema.json
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
title: Invoice
---

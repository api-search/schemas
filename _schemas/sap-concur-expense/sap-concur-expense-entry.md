---
description: Schema for an SAP Concur Expense Entry — a single expense line item within an expense report representing a specific transaction such as a meal, hotel, flight, or other business expense.
layout: schema
name: SAP Concur Expense Entry
properties_list:
- description: The unique identifier of the expense entry
  name: ID
  type: string
- description: The parent expense report ID that contains this entry
  name: ReportID
  type: string
- description: Expense category code (e.g., BUSML for Business Meal, AIRFR for Airfare, HOTEL for Hotel)
  name: ExpenseTypeCode
  type: string
- description: Human-readable expense type label
  name: ExpenseTypeName
  type: string
- description: ISO 8601 date when the expense transaction occurred
  name: TransactionDate
  type: string
- description: Expense amount in the original transaction currency
  name: TransactionAmount
  type: number
- description: ISO 4217 currency code for the transaction
  name: TransactionCurrencyCode
  type: string
- description: Expense amount converted and posted in the report currency
  name: PostedAmount
  type: number
- description: Exchange rate used to convert transaction currency to report currency
  name: ExchangeRate
  type: number
- description: Description of the business reason for this expense
  name: BusinessPurpose
  type: string
- description: Name of the vendor, merchant, or service provider
  name: VendorDescription
  type: string
- description: City or location where the expense was incurred
  name: LocationName
  type: string
- description: Whether this entry has been broken down into itemized sub-entries
  name: IsItemized
  type: boolean
- description: Whether VAT/GST tax applies to this entry
  name: HasVAT
  type: boolean
- description: ID of the receipt image attached to this entry
  name: ReceiptImageID
  type: string
- description: Whether a receipt has been received and attached
  name: ReceiptReceived
  type: boolean
- description: Whether a receipt is required by expense policy for this entry
  name: ReceiptRequired
  type: boolean
- description: Additional notes or comments from the expense owner
  name: Comment
  type: string
- description: Full URI for the expense entry resource
  name: URI
  type: string
provider_name: SAP Concur Expense
provider_slug: sap-concur-expense
schema_file: json-schema/sap-concur-expense-entry-schema.json
slug: sap-concur-expense-entry
source_filename: sap-concur-expense-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/sap-concur-expense/json-schema/sap-concur-expense-entry-schema.json\",\n  \"title\": \"SAP Concur Expense Entry\",\n  \"description\": \"Schema for an SAP Concur Expense Entry — a single expense line item within an expense report representing a specific transaction such as a meal, hotel, flight, or other business expense.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the expense entry\"\n    },\n    \"ReportID\": {\n      \"type\": \"string\",\n      \"description\": \"The parent expense report ID that contains this entry\"\n    },\n    \"ExpenseTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Expense category code (e.g., BUSML for Business Meal, AIRFR for Airfare, HOTEL for Hotel)\"\n    },\n    \"ExpenseTypeName\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Human-readable expense type label\"\n    },\n    \"TransactionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"ISO 8601 date when the expense transaction occurred\"\n    },\n    \"TransactionAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Expense amount in the original transaction currency\"\n    },\n    \"TransactionCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the transaction\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"PostedAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Expense amount converted and posted in the report currency\"\n    },\n    \"ExchangeRate\": {\n      \"type\": \"number\",\n      \"description\": \"Exchange rate used to convert transaction currency to report currency\"\n    },\n    \"BusinessPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the business reason for\
  \ this expense\",\n      \"maxLength\": 255\n    },\n    \"VendorDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the vendor, merchant, or service provider\"\n    },\n    \"LocationName\": {\n      \"type\": \"string\",\n      \"description\": \"City or location where the expense was incurred\"\n    },\n    \"IsItemized\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this entry has been broken down into itemized sub-entries\"\n    },\n    \"HasVAT\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether VAT/GST tax applies to this entry\"\n    },\n    \"ReceiptImageID\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the receipt image attached to this entry\"\n    },\n    \"ReceiptReceived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a receipt has been received and attached\"\n    },\n    \"ReceiptRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a receipt\
  \ is required by expense policy for this entry\"\n    },\n    \"Comment\": {\n      \"type\": \"string\",\n      \"description\": \"Additional notes or comments from the expense owner\",\n      \"maxLength\": 500\n    },\n    \"URI\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Full URI for the expense entry resource\"\n    }\n  },\n  \"required\": [\"ReportID\", \"ExpenseTypeCode\", \"TransactionDate\", \"TransactionAmount\", \"TransactionCurrencyCode\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/json-schema/sap-concur-expense-entry-schema.json
tags:
- Expense Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
- SAP
- Travel
title: SAP Concur Expense Entry
---

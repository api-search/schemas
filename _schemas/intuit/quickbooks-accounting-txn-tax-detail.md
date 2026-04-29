---
description: Tax details for a transaction
layout: schema
name: TxnTaxDetail
properties_list:
- description: Total tax calculated for the transaction
  name: TotalTax
  type: number
- description: ''
  name: TaxLine
  type: array
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-txn-tax-detail-schema.json
slug: quickbooks-accounting-txn-tax-detail
source_filename: quickbooks-accounting-txn-tax-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TxnTaxDetail\",\n  \"type\": \"object\",\n  \"description\": \"Tax details for a transaction\",\n  \"properties\": {\n    \"TotalTax\": {\n      \"type\": \"number\",\n      \"description\": \"Total tax calculated for the transaction\"\n    },\n    \"TaxLine\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-txn-tax-detail-schema.json
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
title: TxnTaxDetail
---

---
description: A line item on a payment showing how it is applied
layout: schema
name: PaymentLine
properties_list:
- description: Amount to apply from this payment
  name: Amount
  type: number
- description: ''
  name: LinkedTxn
  type: array
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-payment-line-schema.json
slug: quickbooks-accounting-payment-line
source_filename: quickbooks-accounting-payment-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentLine\",\n  \"type\": \"object\",\n  \"description\": \"A line item on a payment showing how it is applied\",\n  \"properties\": {\n    \"Amount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount to apply from this payment\"\n    },\n    \"LinkedTxn\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-payment-line-schema.json
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
title: PaymentLine
---

---
description: Detail for a sales item line
layout: schema
name: SalesItemLineDetail
properties_list:
- description: Unit price of the item
  name: UnitPrice
  type: number
- description: The discount rate as a percentage (for discount lines)
  name: RatePercent
  type: number
- description: Number of items for the line
  name: Qty
  type: number
- description: Date the service was performed
  name: ServiceDate
  type: string
- description: Discount amount applied to the line
  name: DiscountAmt
  type: number
- description: Discount rate as a percentage
  name: DiscountRate
  type: number
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-sales-item-line-detail-schema.json
slug: quickbooks-accounting-sales-item-line-detail
source_filename: quickbooks-accounting-sales-item-line-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesItemLineDetail\",\n  \"type\": \"object\",\n  \"description\": \"Detail for a sales item line\",\n  \"properties\": {\n    \"UnitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Unit price of the item\"\n    },\n    \"RatePercent\": {\n      \"type\": \"number\",\n      \"description\": \"The discount rate as a percentage (for discount lines)\"\n    },\n    \"Qty\": {\n      \"type\": \"number\",\n      \"description\": \"Number of items for the line\"\n    },\n    \"ServiceDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the service was performed\"\n    },\n    \"DiscountAmt\": {\n      \"type\": \"number\",\n      \"description\": \"Discount amount applied to the line\"\n    },\n    \"DiscountRate\": {\n      \"type\": \"number\",\n      \"description\": \"Discount rate as a percentage\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-sales-item-line-detail-schema.json
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
title: SalesItemLineDetail
---

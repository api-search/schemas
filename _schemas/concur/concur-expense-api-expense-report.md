---
description: An expense report containing expense entries.
layout: schema
name: ExpenseReport
properties_list:
- description: Unique identifier for the expense report.
  name: reportId
  type: string
- description: Name of the expense report.
  name: reportName
  type: string
- description: Full name of the report owner.
  name: ownerName
  type: string
- description: Business purpose for the expenses.
  name: businessPurpose
  type: string
- description: Date the report was submitted.
  name: submitDate
  type: string
- description: ''
  name: approvalStatus
  type: string
- description: Total amount of all expenses.
  name: total
  type: number
- description: ISO 4217 currency code.
  name: currencyCode
  type: string
- description: ISO country code.
  name: countryCode
  type: string
- description: Date of the report.
  name: reportDate
  type: string
provider_name: SAP Concur
provider_slug: concur
schema_file: json-schema/concur-expense-api-expense-report-schema.json
slug: concur-expense-api-expense-report
source_filename: concur-expense-api-expense-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/json-schema/concur-expense-api-expense-report-schema.json\",\n  \"title\": \"ExpenseReport\",\n  \"description\": \"An expense report containing expense entries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportId\": { \"type\": \"string\", \"description\": \"Unique identifier for the expense report.\", \"example\": \"500123\" },\n    \"reportName\": { \"type\": \"string\", \"description\": \"Name of the expense report.\", \"example\": \"Q1 Travel Expenses\" },\n    \"ownerName\": { \"type\": \"string\", \"description\": \"Full name of the report owner.\", \"example\": \"Jane Smith\" },\n    \"businessPurpose\": { \"type\": \"string\", \"description\": \"Business purpose for the expenses.\" },\n    \"submitDate\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Date the report was submitted.\"\
  \ },\n    \"approvalStatus\": { \"type\": \"string\", \"enum\": [\"NOT_SUBMITTED\", \"SUBMITTED\", \"APPROVED\", \"SENT_BACK\", \"RECALLED\"] },\n    \"total\": { \"type\": \"number\", \"format\": \"double\", \"description\": \"Total amount of all expenses.\" },\n    \"currencyCode\": { \"type\": \"string\", \"description\": \"ISO 4217 currency code.\" },\n    \"countryCode\": { \"type\": \"string\", \"description\": \"ISO country code.\" },\n    \"reportDate\": { \"type\": \"string\", \"format\": \"date\", \"description\": \"Date of the report.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/json-schema/concur-expense-api-expense-report-schema.json
tags:
- Expense Management
- Finance
- Invoice
- SAP
- Travel
title: ExpenseReport
---

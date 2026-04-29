---
description: Request body for creating a new expense report
layout: schema
name: NewReport
properties_list:
- description: The name or title of the expense report
  name: name
  type: string
- description: The business justification for the expenses
  name: businessPurpose
  type: string
- description: The date of the report (YYYY-MM-DD)
  name: reportDate
  type: string
- description: The start date of the reporting period
  name: startDate
  type: string
- description: The end date of the reporting period
  name: endDate
  type: string
- description: ISO 4217 three-letter currency code for the report
  name: currencyCode
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: countryCode
  type: string
- description: ISO 3166-2 subdivision code (state/province)
  name: countrySubDivisionCode
  type: string
- description: The identifier of the expense policy to apply
  name: policyId
  type: string
- description: Custom field values for the report header
  name: customData
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-new-report-schema.json
slug: sap-concur-expense-new-report
source_filename: sap-concur-expense-new-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NewReport\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new expense report\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name or title of the expense report\"\n    },\n    \"businessPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"The business justification for the expenses\"\n    },\n    \"reportDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the report (YYYY-MM-DD)\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"The start date of the reporting period\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"The end date of the reporting period\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code for the report\"\n    },\n\
  \    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    },\n    \"countrySubDivisionCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-2 subdivision code (state/province)\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the expense policy to apply\"\n    },\n    \"customData\": {\n      \"type\": \"array\",\n      \"description\": \"Custom field values for the report header\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-new-report-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: NewReport
---

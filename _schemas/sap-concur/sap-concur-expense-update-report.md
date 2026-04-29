---
description: JSON Merge Patch body for updating an unsubmitted report. All fields from NewReport are updatable.
layout: schema
name: UpdateReport
properties_list:
- description: The name or title of the expense report
  name: name
  type: string
- description: The business justification for the expenses
  name: businessPurpose
  type: string
- description: ''
  name: reportDate
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: countryCode
  type: string
- description: ''
  name: countrySubDivisionCode
  type: string
- description: ''
  name: policyId
  type: string
- description: ''
  name: customData
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-update-report-schema.json
slug: sap-concur-expense-update-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateReport\",\n  \"type\": \"object\",\n  \"description\": \"JSON Merge Patch body for updating an unsubmitted report. All fields from NewReport are updatable.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name or title of the expense report\"\n    },\n    \"businessPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"The business justification for the expenses\"\n    },\n    \"reportDate\": {\n      \"type\": \"string\"\n    },\n    \"startDate\": {\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\"\n    },\n    \"countrySubDivisionCode\": {\n      \"type\": \"string\"\n    },\n    \"policyId\": {\n      \"type\": \"string\"\n    },\n    \"customData\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-update-report-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: UpdateReport
---

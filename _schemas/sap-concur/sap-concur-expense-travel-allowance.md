---
description: Travel allowance (per diem) data associated with an expense
layout: schema
name: TravelAllowance
properties_list:
- description: Whether this expense is part of a travel allowance
  name: isExpensePartOfTravelAllowance
  type: boolean
- description: Identifier of the daily travel allowance
  name: dailyTravelAllowanceId
  type: string
- description: The daily allowance limit amount
  name: dailyLimitAmount
  type: number
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-travel-allowance-schema.json
slug: sap-concur-expense-travel-allowance
source_filename: sap-concur-expense-travel-allowance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TravelAllowance\",\n  \"type\": \"object\",\n  \"description\": \"Travel allowance (per diem) data associated with an expense\",\n  \"properties\": {\n    \"isExpensePartOfTravelAllowance\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this expense is part of a travel allowance\"\n    },\n    \"dailyTravelAllowanceId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the daily travel allowance\"\n    },\n    \"dailyLimitAmount\": {\n      \"type\": \"number\",\n      \"description\": \"The daily allowance limit amount\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-travel-allowance-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: TravelAllowance
---

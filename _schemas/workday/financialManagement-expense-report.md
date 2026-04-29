---
description: ''
layout: schema
name: ExpenseReport
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: totalAmount
  type: number
- description: Status of the report (e.g., Draft, Submitted, Approved, Paid).
  name: status
  type: string
- description: ''
  name: memo
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/financialManagement-expense-report-schema.json
slug: financialManagement-expense-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExpenseReport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the report (e.g., Draft, Submitted, Approved, Paid).\"\n    },\n    \"memo\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/financialManagement-expense-report-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: ExpenseReport
---

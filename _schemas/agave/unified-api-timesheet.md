---
description: An employee timesheet entry.
layout: schema
name: Timesheet
properties_list:
- description: Timesheet identifier.
  name: id
  type: string
- description: Employee identifier.
  name: employee_id
  type: string
- description: Associated project identifier.
  name: project_id
  type: string
- description: Associated cost code.
  name: cost_code_id
  type: string
- description: Timesheet date.
  name: date
  type: string
- description: Regular hours worked.
  name: regular_hours
  type: number
- description: Overtime hours worked.
  name: overtime_hours
  type: number
- description: Hourly pay rate in USD.
  name: pay_rate
  type: number
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-timesheet-schema.json
slug: unified-api-timesheet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-timesheet-schema.json\",\n  \"title\": \"Timesheet\",\n  \"description\": \"An employee timesheet entry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Timesheet identifier.\",\n      \"example\": \"ts-990011\"\n    },\n    \"employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employee identifier.\",\n      \"example\": \"emp-123456\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated project identifier.\",\n      \"example\": \"proj-500123\"\n    },\n    \"cost_code_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated cost code.\",\n      \"example\": \"cc-445566\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\
  ,\n      \"description\": \"Timesheet date.\",\n      \"example\": \"2025-03-15\"\n    },\n    \"regular_hours\": {\n      \"type\": \"number\",\n      \"description\": \"Regular hours worked.\",\n      \"example\": 8.0\n    },\n    \"overtime_hours\": {\n      \"type\": \"number\",\n      \"description\": \"Overtime hours worked.\",\n      \"example\": 2.0\n    },\n    \"pay_rate\": {\n      \"type\": \"number\",\n      \"description\": \"Hourly pay rate in USD.\",\n      \"example\": 45.0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-timesheet-schema.json
tags:
- Accounting
- Construction
- Integration
title: Timesheet
---

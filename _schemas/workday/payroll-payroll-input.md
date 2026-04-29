---
description: ''
layout: schema
name: PayrollInput
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: inputType
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: comment
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/payroll-payroll-input-schema.json
slug: payroll-payroll-input
source_filename: payroll-payroll-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PayrollInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"inputType\": {\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"type\": \"number\"\n    },\n    \"startDate\": {\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/payroll-payroll-input-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: PayrollInput
---

---
description: ''
layout: schema
name: PaySlip
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: payPeriodStartDate
  type: string
- description: ''
  name: payPeriodEndDate
  type: string
- description: ''
  name: payDate
  type: string
- description: ''
  name: grossPay
  type: number
- description: ''
  name: netPay
  type: number
- description: ''
  name: totalDeductions
  type: number
- description: ''
  name: totalTaxes
  type: number
provider_name: Workday
provider_slug: workday
schema_file: json-schema/payroll-pay-slip-schema.json
slug: payroll-pay-slip
source_filename: payroll-pay-slip-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaySlip\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"payPeriodStartDate\": {\n      \"type\": \"string\"\n    },\n    \"payPeriodEndDate\": {\n      \"type\": \"string\"\n    },\n    \"payDate\": {\n      \"type\": \"string\"\n    },\n    \"grossPay\": {\n      \"type\": \"number\"\n    },\n    \"netPay\": {\n      \"type\": \"number\"\n    },\n    \"totalDeductions\": {\n      \"type\": \"number\"\n    },\n    \"totalTaxes\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/payroll-pay-slip-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: PaySlip
---

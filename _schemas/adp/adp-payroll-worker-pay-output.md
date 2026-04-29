---
description: ''
layout: schema
name: WorkerPayOutput
properties_list:
- description: ''
  name: associateOID
  type: string
- description: ''
  name: workerID
  type: object
- description: ''
  name: payStatementID
  type: string
- description: ''
  name: payDate
  type: string
- description: ''
  name: regularEarnings
  type: array
- description: ''
  name: overtimeEarnings
  type: array
- description: ''
  name: otherEarnings
  type: array
- description: ''
  name: deductions
  type: array
- description: ''
  name: taxes
  type: array
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-payroll-worker-pay-output-schema.json
slug: adp-payroll-worker-pay-output
source_filename: adp-payroll-worker-pay-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkerPayOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"associateOID\": {\n      \"type\": \"string\"\n    },\n    \"workerID\": {\n      \"type\": \"object\"\n    },\n    \"payStatementID\": {\n      \"type\": \"string\"\n    },\n    \"payDate\": {\n      \"type\": \"string\"\n    },\n    \"regularEarnings\": {\n      \"type\": \"array\"\n    },\n    \"overtimeEarnings\": {\n      \"type\": \"array\"\n    },\n    \"otherEarnings\": {\n      \"type\": \"array\"\n    },\n    \"deductions\": {\n      \"type\": \"array\"\n    },\n    \"taxes\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-payroll-worker-pay-output-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: WorkerPayOutput
---

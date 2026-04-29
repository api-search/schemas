---
description: ''
layout: schema
name: PayrollOutputSummary
properties_list:
- description: ''
  name: payrollOutputID
  type: string
- description: ''
  name: payrollScheduleReference
  type: object
- description: ''
  name: payrollStatusCode
  type: object
- description: ''
  name: workerCount
  type: integer
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-payroll-payroll-output-summary-schema.json
slug: adp-payroll-payroll-output-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PayrollOutputSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"payrollOutputID\": {\n      \"type\": \"string\"\n    },\n    \"payrollScheduleReference\": {\n      \"type\": \"object\"\n    },\n    \"payrollStatusCode\": {\n      \"type\": \"object\"\n    },\n    \"workerCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-payroll-payroll-output-summary-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: PayrollOutputSummary
---

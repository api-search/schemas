---
description: ''
layout: schema
name: PayrollOutput
properties_list:
- description: ''
  name: payrollOutputID
  type: string
- description: ''
  name: payrollScheduleReference
  type: object
- description: ''
  name: payrollSummary
  type: object
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-payroll-payroll-output-schema.json
slug: adp-payroll-payroll-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PayrollOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"payrollOutputID\": {\n      \"type\": \"string\"\n    },\n    \"payrollScheduleReference\": {\n      \"type\": \"object\"\n    },\n    \"payrollSummary\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-payroll-payroll-output-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: PayrollOutput
---

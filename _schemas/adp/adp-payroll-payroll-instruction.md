---
description: ''
layout: schema
name: PayrollInstruction
properties_list:
- description: ''
  name: instructionID
  type: string
- description: ''
  name: associateOID
  type: string
- description: ''
  name: instructionTypeCode
  type: string
- description: ''
  name: effectiveDate
  type: string
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-payroll-payroll-instruction-schema.json
slug: adp-payroll-payroll-instruction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PayrollInstruction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instructionID\": {\n      \"type\": \"string\"\n    },\n    \"associateOID\": {\n      \"type\": \"string\"\n    },\n    \"instructionTypeCode\": {\n      \"type\": \"string\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-payroll-payroll-instruction-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: PayrollInstruction
---

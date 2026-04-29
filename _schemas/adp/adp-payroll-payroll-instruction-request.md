---
description: ''
layout: schema
name: PayrollInstructionRequest
properties_list:
- description: ''
  name: associateOID
  type: string
- description: ''
  name: instructionTypeCode
  type: string
- description: ''
  name: effectiveDate
  type: string
- description: ''
  name: description
  type: string
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-payroll-payroll-instruction-request-schema.json
slug: adp-payroll-payroll-instruction-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PayrollInstructionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"associateOID\": {\n      \"type\": \"string\"\n    },\n    \"instructionTypeCode\": {\n      \"type\": \"string\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-payroll-payroll-instruction-request-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: PayrollInstructionRequest
---

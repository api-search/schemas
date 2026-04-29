---
description: ''
layout: schema
name: PayrollRun
properties_list:
- description: Payroll action identifier
  name: payrollActionId
  type: integer
- description: Payroll identifier
  name: payrollId
  type: integer
- description: Action type (R=Run, Q=QuickPay, etc.)
  name: actionType
  type: string
- description: Action status
  name: actionStatus
  type: string
- description: ''
  name: effectiveDate
  type: string
- description: ''
  name: dateEarned
  type: string
- description: ''
  name: periodOfServiceId
  type: integer
- description: ''
  name: businessGroupId
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-payroll-run-schema.json
slug: human-resources-payroll-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PayrollRun\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"payrollActionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Payroll action identifier\"\n    },\n    \"payrollId\": {\n      \"type\": \"integer\",\n      \"description\": \"Payroll identifier\"\n    },\n    \"actionType\": {\n      \"type\": \"string\",\n      \"description\": \"Action type (R=Run, Q=QuickPay, etc.)\"\n    },\n    \"actionStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Action status\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\"\n    },\n    \"dateEarned\": {\n      \"type\": \"string\"\n    },\n    \"periodOfServiceId\": {\n      \"type\": \"integer\"\n    },\n    \"businessGroupId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-payroll-run-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: PayrollRun
---

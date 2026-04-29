---
description: ''
layout: schema
name: Payroll
properties_list:
- description: Payroll identifier
  name: payrollId
  type: integer
- description: Payroll name
  name: payrollName
  type: string
- description: Payroll period type
  name: periodType
  type: string
- description: Number of years defined
  name: numberOfYears
  type: integer
- description: ''
  name: firstPeriodEndDate
  type: string
- description: ''
  name: effectiveStartDate
  type: string
- description: ''
  name: effectiveEndDate
  type: string
- description: ''
  name: businessGroupId
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-payroll-schema.json
slug: human-resources-payroll
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Payroll\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"payrollId\": {\n      \"type\": \"integer\",\n      \"description\": \"Payroll identifier\"\n    },\n    \"payrollName\": {\n      \"type\": \"string\",\n      \"description\": \"Payroll name\"\n    },\n    \"periodType\": {\n      \"type\": \"string\",\n      \"description\": \"Payroll period type\"\n    },\n    \"numberOfYears\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of years defined\"\n    },\n    \"firstPeriodEndDate\": {\n      \"type\": \"string\"\n    },\n    \"effectiveStartDate\": {\n      \"type\": \"string\"\n    },\n    \"effectiveEndDate\": {\n      \"type\": \"string\"\n    },\n    \"businessGroupId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-payroll-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Payroll
---

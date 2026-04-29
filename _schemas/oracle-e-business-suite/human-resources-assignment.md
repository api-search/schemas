---
description: ''
layout: schema
name: Assignment
properties_list:
- description: Assignment identifier
  name: assignmentId
  type: integer
- description: Assignment number
  name: assignmentNumber
  type: string
- description: Assignment type
  name: assignmentType
  type: string
- description: Whether this is the primary assignment
  name: primaryFlag
  type: string
- description: Job identifier
  name: jobId
  type: integer
- description: Job name
  name: jobName
  type: string
- description: Position identifier
  name: positionId
  type: integer
- description: Position name
  name: positionName
  type: string
- description: Grade identifier
  name: gradeId
  type: integer
- description: Grade name
  name: gradeName
  type: string
- description: Organization identifier
  name: organizationId
  type: integer
- description: Organization name
  name: organizationName
  type: string
- description: Location identifier
  name: locationId
  type: integer
- description: Location code
  name: locationCode
  type: string
- description: Supervisor person identifier
  name: supervisorId
  type: integer
- description: Payroll identifier
  name: payrollId
  type: integer
- description: Employment category
  name: employmentCategory
  type: string
- description: Normal working hours
  name: normalHours
  type: number
- description: Hours frequency
  name: frequency
  type: string
- description: ''
  name: effectiveStartDate
  type: string
- description: ''
  name: effectiveEndDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-assignment-schema.json
slug: human-resources-assignment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Assignment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assignmentId\": {\n      \"type\": \"integer\",\n      \"description\": \"Assignment identifier\"\n    },\n    \"assignmentNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Assignment number\"\n    },\n    \"assignmentType\": {\n      \"type\": \"string\",\n      \"description\": \"Assignment type\"\n    },\n    \"primaryFlag\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this is the primary assignment\"\n    },\n    \"jobId\": {\n      \"type\": \"integer\",\n      \"description\": \"Job identifier\"\n    },\n    \"jobName\": {\n      \"type\": \"string\",\n      \"description\": \"Job name\"\n    },\n    \"positionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Position identifier\"\n    },\n    \"positionName\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Position name\"\n    },\n    \"gradeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Grade identifier\"\n    },\n    \"gradeName\": {\n      \"type\": \"string\",\n      \"description\": \"Grade name\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"organizationName\": {\n      \"type\": \"string\",\n      \"description\": \"Organization name\"\n    },\n    \"locationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Location identifier\"\n    },\n    \"locationCode\": {\n      \"type\": \"string\",\n      \"description\": \"Location code\"\n    },\n    \"supervisorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Supervisor person identifier\"\n    },\n    \"payrollId\": {\n      \"type\": \"integer\",\n      \"description\": \"Payroll identifier\"\n    },\n    \"employmentCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Employment category\"\
  \n    },\n    \"normalHours\": {\n      \"type\": \"number\",\n      \"description\": \"Normal working hours\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Hours frequency\"\n    },\n    \"effectiveStartDate\": {\n      \"type\": \"string\"\n    },\n    \"effectiveEndDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-assignment-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Assignment
---

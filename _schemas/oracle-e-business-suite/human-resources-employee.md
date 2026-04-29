---
description: ''
layout: schema
name: Employee
properties_list:
- description: Person identifier
  name: personId
  type: integer
- description: Employee number
  name: employeeNumber
  type: string
- description: Title (Mr., Mrs., etc.)
  name: title
  type: string
- description: First name
  name: firstName
  type: string
- description: Middle name(s)
  name: middleNames
  type: string
- description: Last name
  name: lastName
  type: string
- description: Full name (derived)
  name: fullName
  type: string
- description: Preferred name
  name: knownAs
  type: string
- description: Email address
  name: emailAddress
  type: string
- description: Gender
  name: sex
  type: string
- description: Date of birth
  name: dateOfBirth
  type: string
- description: National identifier (e.g., SSN)
  name: nationalIdentifier
  type: string
- description: Nationality code
  name: nationality
  type: string
- description: Marital status
  name: maritalStatus
  type: string
- description: Record effective start date (date-tracked)
  name: effectiveStartDate
  type: string
- description: Record effective end date (date-tracked)
  name: effectiveEndDate
  type: string
- description: Original hire date
  name: hireDate
  type: string
- description: ''
  name: currentEmployeeFlag
  type: string
- description: Business group identifier
  name: businessGroupId
  type: integer
- description: ''
  name: addresses
  type: array
- description: ''
  name: phones
  type: array
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-employee-schema.json
slug: human-resources-employee
source_filename: human-resources-employee-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Employee\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"personId\": {\n      \"type\": \"integer\",\n      \"description\": \"Person identifier\"\n    },\n    \"employeeNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Employee number\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title (Mr., Mrs., etc.)\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name\"\n    },\n    \"middleNames\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name(s)\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name\"\n    },\n    \"fullName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name (derived)\"\n    },\n    \"knownAs\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred name\"\n    },\n    \"emailAddress\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Email address\"\n    },\n    \"sex\": {\n      \"type\": \"string\",\n      \"description\": \"Gender\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\",\n      \"description\": \"Date of birth\"\n    },\n    \"nationalIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"National identifier (e.g., SSN)\"\n    },\n    \"nationality\": {\n      \"type\": \"string\",\n      \"description\": \"Nationality code\"\n    },\n    \"maritalStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Marital status\"\n    },\n    \"effectiveStartDate\": {\n      \"type\": \"string\",\n      \"description\": \"Record effective start date (date-tracked)\"\n    },\n    \"effectiveEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"Record effective end date (date-tracked)\"\n    },\n    \"hireDate\": {\n      \"type\": \"string\",\n      \"description\": \"Original hire date\"\n    },\n    \"\
  currentEmployeeFlag\": {\n      \"type\": \"string\"\n    },\n    \"businessGroupId\": {\n      \"type\": \"integer\",\n      \"description\": \"Business group identifier\"\n    },\n    \"addresses\": {\n      \"type\": \"array\"\n    },\n    \"phones\": {\n      \"type\": \"array\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-employee-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Employee
---

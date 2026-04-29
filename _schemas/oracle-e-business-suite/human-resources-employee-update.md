---
description: ''
layout: schema
name: EmployeeUpdate
properties_list:
- description: Date-track effective date for the update
  name: effectiveDate
  type: string
- description: Date-track update mode
  name: dateTrackUpdateMode
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: middleNames
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: knownAs
  type: string
- description: ''
  name: emailAddress
  type: string
- description: ''
  name: maritalStatus
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-employee-update-schema.json
slug: human-resources-employee-update
source_filename: human-resources-employee-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmployeeUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date-track effective date for the update\"\n    },\n    \"dateTrackUpdateMode\": {\n      \"type\": \"string\",\n      \"description\": \"Date-track update mode\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"middleNames\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"knownAs\": {\n      \"type\": \"string\"\n    },\n    \"emailAddress\": {\n      \"type\": \"string\"\n    },\n    \"maritalStatus\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-employee-update-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: EmployeeUpdate
---

---
description: ''
layout: schema
name: WorkAssignment
properties_list:
- description: ''
  name: itemID
  type: string
- description: ''
  name: primaryIndicator
  type: boolean
- description: ''
  name: hireDate
  type: string
- description: ''
  name: assignmentStatus
  type: object
- description: ''
  name: positionID
  type: string
- description: ''
  name: jobCode
  type: object
- description: ''
  name: jobTitle
  type: string
- description: ''
  name: standardHours
  type: object
- description: ''
  name: annualBaseRemuneration
  type: object
- description: ''
  name: homeOrganizationalUnits
  type: array
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-workers-work-assignment-schema.json
slug: adp-workers-work-assignment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkAssignment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"itemID\": {\n      \"type\": \"string\"\n    },\n    \"primaryIndicator\": {\n      \"type\": \"boolean\"\n    },\n    \"hireDate\": {\n      \"type\": \"string\"\n    },\n    \"assignmentStatus\": {\n      \"type\": \"object\"\n    },\n    \"positionID\": {\n      \"type\": \"string\"\n    },\n    \"jobCode\": {\n      \"type\": \"object\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\"\n    },\n    \"standardHours\": {\n      \"type\": \"object\"\n    },\n    \"annualBaseRemuneration\": {\n      \"type\": \"object\"\n    },\n    \"homeOrganizationalUnits\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-workers-work-assignment-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: WorkAssignment
---

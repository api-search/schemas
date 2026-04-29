---
description: Complete skills matrix for an employee
layout: schema
name: EmployeeSkillsMatrix
properties_list:
- description: Employee identifier
  name: employeeId
  type: string
- description: Employee name
  name: employeeName
  type: string
- description: Current job role
  name: role
  type: string
- description: ''
  name: skills
  type: array
- description: Overall skill completion percentage
  name: overallCompletion
  type: integer
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-employee-skills-matrix-schema.json
slug: acadia-employee-skills-matrix
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-employee-skills-matrix-schema.json\",\n  \"title\": \"EmployeeSkillsMatrix\",\n  \"description\": \"Complete skills matrix for an employee\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"employeeId\": {\n      \"type\": \"string\",\n      \"description\": \"Employee identifier\",\n      \"example\": \"emp-ghi789\"\n    },\n    \"employeeName\": {\n      \"type\": \"string\",\n      \"description\": \"Employee name\",\n      \"example\": \"Jane Smith\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Current job role\",\n      \"example\": \"Machine Operator\"\n    },\n    \"skills\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SkillRecord\"\n      }\n    },\n    \"overallCompletion\": {\n      \"type\": \"integer\",\n\
  \      \"description\": \"Overall skill completion percentage\",\n      \"example\": 87\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-employee-skills-matrix-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: EmployeeSkillsMatrix
---

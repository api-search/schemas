---
description: An employee in the organization
layout: schema
name: Employee
properties_list:
- description: Unique employee identifier
  name: id
  type: string
- description: Employee full name
  name: name
  type: string
- description: Employee email address
  name: email
  type: string
- description: Department name
  name: department
  type: string
- description: Job role name
  name: role
  type: string
- description: Overall training completion percentage
  name: trainingCompletion
  type: integer
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-employee-schema.json
slug: acadia-employee
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-employee-schema.json\",\n  \"title\": \"Employee\",\n  \"description\": \"An employee in the organization\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique employee identifier\",\n      \"example\": \"emp-ghi789\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Employee full name\",\n      \"example\": \"Jane Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Employee email address\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department name\",\n      \"example\": \"Production\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Job role name\",\n      \"example\": \"Machine Operator\"\n    },\n    \"trainingCompletion\": {\n      \"type\": \"integer\",\n      \"description\": \"Overall training completion percentage\",\n      \"example\": 87\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-employee-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: Employee
---

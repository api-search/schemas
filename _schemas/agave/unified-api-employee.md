---
description: An employee record.
layout: schema
name: Employee
properties_list:
- description: Employee identifier.
  name: id
  type: string
- description: Employee first name.
  name: first_name
  type: string
- description: Employee last name.
  name: last_name
  type: string
- description: Employee email address.
  name: email
  type: string
- description: Employee job title.
  name: title
  type: string
- description: Employment status.
  name: status
  type: string
- description: Date of hire.
  name: hire_date
  type: string
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-employee-schema.json
slug: unified-api-employee
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-employee-schema.json\",\n  \"title\": \"Employee\",\n  \"description\": \"An employee record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Employee identifier.\",\n      \"example\": \"emp-123456\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Employee first name.\",\n      \"example\": \"John\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Employee last name.\",\n      \"example\": \"Doe\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Employee email address.\",\n      \"example\": \"john.doe@contractor.com\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Employee job title.\",\n  \
  \    \"example\": \"Project Manager\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Employment status.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"terminated\"\n      ],\n      \"example\": \"active\"\n    },\n    \"hire_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of hire.\",\n      \"example\": \"2020-06-01\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-employee-schema.json
tags:
- Accounting
- Construction
- Integration
title: Employee
---

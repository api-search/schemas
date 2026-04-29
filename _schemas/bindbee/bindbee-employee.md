---
description: A normalized employee record from a connected HRIS system.
layout: schema
name: Employee
properties_list:
- description: Bindbee employee ID.
  name: id
  type: string
- description: Employee first name.
  name: first_name
  type: string
- description: Employee last name.
  name: last_name
  type: string
- description: Employee work email.
  name: email
  type: string
- description: Job title.
  name: job_title
  type: string
- description: Department name.
  name: department
  type: string
- description: Employment status.
  name: employment_status
  type: string
- description: Employment start date.
  name: start_date
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-employee-schema.json
slug: bindbee-employee
source_filename: bindbee-employee-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Employee\",\n  \"type\": \"object\",\n  \"description\": \"A normalized employee record from a connected HRIS system.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Bindbee employee ID.\",\n      \"example\": \"emp-abc123\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Employee first name.\",\n      \"example\": \"Jane\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Employee last name.\",\n      \"example\": \"Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Employee work email.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"job_title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title.\",\n      \"example\": \"Software Engineer\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Department name.\",\n      \"example\": \"Engineering\"\n    },\n    \"employment_status\": {\n      \"type\": \"string\",\n      \"description\": \"Employment status.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"terminated\"\n      ],\n      \"example\": \"active\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Employment start date.\",\n      \"example\": \"2022-03-15\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-employee-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: Employee
---

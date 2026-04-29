---
description: An organizational department.
layout: schema
name: Department
properties_list:
- description: Unique identifier of the department.
  name: _id
  type: string
- description: Name of the department.
  name: name
  type: string
- description: ID of the department manager.
  name: managerId
  type: string
- description: ID of the parent department if hierarchical.
  name: parentId
  type: string
provider_name: Absence.io
provider_slug: absence-io
schema_file: json-schema/department-schema.json
slug: department
source_filename: department-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/department-schema.json\",\n  \"title\": \"Department\",\n  \"description\": \"An organizational department.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the department.\",\n      \"example\": \"500999\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the department.\",\n      \"example\": \"Engineering\"\n    },\n    \"managerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the department manager.\",\n      \"example\": \"500456\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent department if hierarchical.\",\n      \"example\": \"500000\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/department-schema.json
tags:
- Absences
- Employees
- Leave Management
- HR
title: Department
---

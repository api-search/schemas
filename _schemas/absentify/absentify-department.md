---
description: A department in the absentify workspace.
layout: schema
name: Department
properties_list:
- description: Unique identifier of the department.
  name: id
  type: string
- description: Name of the department.
  name: name
  type: string
- description: Timestamp when the department was created.
  name: createdAt
  type: string
- description: Timestamp when the department was last updated.
  name: updatedAt
  type: string
provider_name: Absentify
provider_slug: absentify
schema_file: json-schema/absentify-department-schema.json
slug: absentify-department
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absentify/main/json-schema/absentify-department-schema.json\",\n  \"title\": \"Department\",\n  \"description\": \"A department in the absentify workspace.\",\n  \"type\": \"object\",\n  \"x-schema-source\": \"openapi-spec\",\n  \"x-provider\": \"absentify\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the department.\",\n      \"example\": \"500999\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the department.\",\n      \"example\": \"Engineering\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the department was created.\",\n      \"example\": \"2025-01-01T00:00:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Timestamp when the department was last updated.\",\n      \"example\": \"2025-06-01T09:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/json-schema/absentify-department-schema.json
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
title: Department
---

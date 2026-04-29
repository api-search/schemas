---
description: A member (employee) in the absentify workspace.
layout: schema
name: Member
properties_list:
- description: Unique identifier of the member.
  name: id
  type: string
- description: Custom identifier for the member.
  name: custom_id
  type: string
- description: Name of the member.
  name: name
  type: string
- description: Email address of the member.
  name: email
  type: string
- description: Current status of the member.
  name: status
  type: string
- description: Whether the member is an admin.
  name: is_admin
  type: boolean
- description: Approval process type for this member.
  name: approval_process
  type: string
- description: Employment start date.
  name: employment_start_date
  type: string
- description: Employment end date if applicable.
  name: employment_end_date
  type: string
- description: Birthday of the member.
  name: birthday
  type: string
- description: Timestamp when the member was created.
  name: createdAt
  type: string
- description: Timestamp when the member was last updated.
  name: updatedAt
  type: string
provider_name: Absentify
provider_slug: absentify
schema_file: json-schema/absentify-member-schema.json
slug: absentify-member
source_filename: absentify-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absentify/main/json-schema/absentify-member-schema.json\",\n  \"title\": \"Member\",\n  \"description\": \"A member (employee) in the absentify workspace.\",\n  \"type\": \"object\",\n  \"x-schema-source\": \"openapi-spec\",\n  \"x-provider\": \"absentify\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the member.\",\n      \"example\": \"500123\"\n    },\n    \"custom_id\": {\n      \"type\": \"string\",\n      \"description\": \"Custom identifier for the member.\",\n      \"example\": \"EMP001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the member.\",\n      \"example\": \"Jane Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the member.\",\n    \
  \  \"example\": \"jsmith@example.com\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the member.\",\n      \"example\": \"ACTIVE\"\n    },\n    \"is_admin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the member is an admin.\",\n      \"example\": false\n    },\n    \"approval_process\": {\n      \"type\": \"string\",\n      \"description\": \"Approval process type for this member.\",\n      \"example\": \"CUSTOM\"\n    },\n    \"employment_start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Employment start date.\",\n      \"example\": \"2024-01-15\"\n    },\n    \"employment_end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"nullable\": true,\n      \"description\": \"Employment end date if applicable.\",\n      \"example\": null\n    },\n    \"birthday\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"nullable\"\
  : true,\n      \"description\": \"Birthday of the member.\",\n      \"example\": \"1990-06-15\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the member was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the member was last updated.\",\n      \"example\": \"2025-06-01T09:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/json-schema/absentify-member-schema.json
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
title: Member
---

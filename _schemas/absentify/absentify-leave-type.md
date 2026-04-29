---
description: A leave type defined in the absentify workspace.
layout: schema
name: LeaveType
properties_list:
- description: Unique identifier of the leave type.
  name: id
  type: string
- description: Name of the leave type.
  name: name
  type: string
- description: Unit for this leave type (days or hours).
  name: leave_unit
  type: string
- description: Color code for this leave type.
  name: color
  type: string
- description: Icon for this leave type.
  name: icon
  type: string
- description: Timestamp when the leave type was created.
  name: createdAt
  type: string
- description: Timestamp when the leave type was last updated.
  name: updatedAt
  type: string
provider_name: Absentify
provider_slug: absentify
schema_file: json-schema/absentify-leave-type-schema.json
slug: absentify-leave-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absentify/main/json-schema/absentify-leave-type-schema.json\",\n  \"title\": \"LeaveType\",\n  \"description\": \"A leave type defined in the absentify workspace.\",\n  \"type\": \"object\",\n  \"x-schema-source\": \"openapi-spec\",\n  \"x-provider\": \"absentify\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the leave type.\",\n      \"example\": \"500789\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the leave type.\",\n      \"example\": \"Vacation\"\n    },\n    \"leave_unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit for this leave type (days or hours).\",\n      \"example\": \"DAYS\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"Color code for this leave type.\",\n      \"example\"\
  : \"#4CAF50\"\n    },\n    \"icon\": {\n      \"type\": \"string\",\n      \"description\": \"Icon for this leave type.\",\n      \"example\": \"beach\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the leave type was created.\",\n      \"example\": \"2025-01-01T00:00:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the leave type was last updated.\",\n      \"example\": \"2025-06-01T09:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/json-schema/absentify-leave-type-schema.json
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
title: LeaveType
---

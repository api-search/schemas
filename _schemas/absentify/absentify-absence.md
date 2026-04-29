---
description: An absence entry for a specific date and member.
layout: schema
name: Absence
properties_list:
- description: Unique identifier of the absence.
  name: id
  type: string
- description: Date of the absence.
  name: date
  type: string
- description: Duration of the absence (0.5 for half day, 1 for full day).
  name: duration
  type: number
- description: ID of the associated leave request.
  name: request_id
  type: string
provider_name: Absentify
provider_slug: absentify
schema_file: json-schema/absentify-absence-schema.json
slug: absentify-absence
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absentify/main/json-schema/absentify-absence-schema.json\",\n  \"title\": \"Absence\",\n  \"description\": \"An absence entry for a specific date and member.\",\n  \"type\": \"object\",\n  \"x-schema-source\": \"openapi-spec\",\n  \"x-provider\": \"absentify\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the absence.\",\n      \"example\": \"500321\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the absence.\",\n      \"example\": \"2025-06-02\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"Duration of the absence (0.5 for half day, 1 for full day).\",\n      \"example\": 1\n    },\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the associated\
  \ leave request.\",\n      \"example\": \"500456\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/json-schema/absentify-absence-schema.json
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
title: Absence
---

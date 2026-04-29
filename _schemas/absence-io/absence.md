---
description: An employee absence record.
layout: schema
name: Absence
properties_list:
- description: Unique identifier of the absence.
  name: _id
  type: string
- description: ID of the user this absence is assigned to.
  name: assignedToId
  type: string
- description: ID of the absence reason type.
  name: reasonId
  type: string
- description: ID of the user who approved this absence.
  name: approverId
  type: string
- description: Start date and time of the absence.
  name: start
  type: string
- description: End date and time of the absence.
  name: end
  type: string
- description: Number of working days covered by the absence.
  name: days
  type: number
- description: 'Absence approval status: 0=pending, 1=approved, 2=declined.'
  name: status
  type: integer
- description: Optional comment or note on the absence.
  name: comment
  type: string
provider_name: Absence.io
provider_slug: absence-io
schema_file: json-schema/absence-schema.json
slug: absence
source_filename: absence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/absence-schema.json\",\n  \"title\": \"Absence\",\n  \"description\": \"An employee absence record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the absence.\",\n      \"example\": \"500123\"\n    },\n    \"assignedToId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user this absence is assigned to.\",\n      \"example\": \"500456\"\n    },\n    \"reasonId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the absence reason type.\",\n      \"example\": \"500789\"\n    },\n    \"approverId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who approved this absence.\",\n      \"example\": \"500654\"\n    },\n    \"start\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Start date and time of the absence.\",\n      \"example\": \"2025-06-01T00:00:00.000Z\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End date and time of the absence.\",\n      \"example\": \"2025-06-05T23:59:59.999Z\"\n    },\n    \"days\": {\n      \"type\": \"number\",\n      \"description\": \"Number of working days covered by the absence.\",\n      \"example\": 5\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"Absence approval status: 0=pending, 1=approved, 2=declined.\",\n      \"example\": 1\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment or note on the absence.\",\n      \"example\": \"Annual leave\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/absence-schema.json
tags:
- Absences
- Employees
- Leave Management
- HR
title: Absence
---

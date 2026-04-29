---
description: An absence reason type (e.g., vacation, sick leave, parental leave).
layout: schema
name: ReasonType
properties_list:
- description: Unique identifier of the reason type.
  name: _id
  type: string
- description: Display name of the absence reason.
  name: name
  type: string
- description: Color code for displaying this absence type in the calendar.
  name: color
  type: string
- description: Whether absences of this type require manager approval.
  name: requiresApproval
  type: boolean
- description: Whether absences of this type count against the employee's allowance.
  name: affectsAllowance
  type: boolean
provider_name: Absence.io
provider_slug: absence-io
schema_file: json-schema/reason-type-schema.json
slug: reason-type
source_filename: reason-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/reason-type-schema.json\",\n  \"title\": \"ReasonType\",\n  \"description\": \"An absence reason type (e.g., vacation, sick leave, parental leave).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the reason type.\",\n      \"example\": \"500789\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the absence reason.\",\n      \"example\": \"Vacation\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"Color code for displaying this absence type in the calendar.\",\n      \"example\": \"#4CAF50\"\n    },\n    \"requiresApproval\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether absences of this type require manager approval.\"\
  ,\n      \"example\": true\n    },\n    \"affectsAllowance\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether absences of this type count against the employee's allowance.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/reason-type-schema.json
tags:
- Absences
- Employees
- Leave Management
- HR
title: ReasonType
---

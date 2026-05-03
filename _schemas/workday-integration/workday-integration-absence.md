---
description: Represents a time off request or leave of absence within the Workday Absence Management system.
layout: schema
name: Absence
properties_list:
- description: The unique Workday identifier for the absence record
  name: id
  type: string
- description: The display name of the absence record
  name: descriptor
  type: string
- description: The worker who requested the absence
  name: worker
  type: object
- description: The type of absence (Vacation, Sick, Personal, etc.)
  name: absenceType
  type: object
- description: The start date of the absence
  name: startDate
  type: string
- description: The end date of the absence
  name: endDate
  type:
  - string
  - 'null'
- description: The duration of the absence in the specified unit
  name: quantity
  type: number
- description: The unit of measurement for the absence quantity
  name: unit
  type: string
- description: The approval status of the absence request
  name: status
  type: string
- description: Optional comment provided with the absence request
  name: comment
  type: string
- description: Whether this is a time off request or leave of absence
  name: absenceCategory
  type: string
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-absence-schema.json
slug: workday-integration-absence
source_filename: workday-integration-absence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/absence\",\n  \"title\": \"Absence\",\n  \"description\": \"Represents a time off request or leave of absence within the Workday Absence Management system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the absence record\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the absence record\"\n    },\n    \"worker\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker who requested the absence\"\n    },\n    \"absenceType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The type of absence (Vacation, Sick, Personal, etc.)\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The start\
  \ date of the absence\"\n    },\n    \"endDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The end date of the absence\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"The duration of the absence in the specified unit\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"enum\": [\"Hours\", \"Days\"],\n      \"description\": \"The unit of measurement for the absence quantity\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Approved\", \"Submitted\", \"Not Submitted\", \"Sent Back\", \"Cancelled\", \"Denied\"],\n      \"description\": \"The approval status of the absence request\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment provided with the absence request\"\n    },\n    \"absenceCategory\": {\n      \"type\": \"string\",\n      \"enum\": [\"Time_Off\", \"Leave_Of_Absence\"],\n      \"description\"\
  : \"Whether this is a time off request or leave of absence\"\n    }\n  },\n  \"required\": [\"id\", \"worker\", \"absenceType\", \"startDate\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-absence-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Absence
---

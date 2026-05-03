---
description: Represents a time block recording worked hours for a worker within the Workday Time Tracking system.
layout: schema
name: Time Block
properties_list:
- description: The unique Workday identifier for the time block
  name: id
  type: string
- description: The display name of the time block
  name: descriptor
  type: string
- description: The worker who recorded the time
  name: worker
  type: object
- description: The date of the time block
  name: date
  type: string
- description: The start time of the time block
  name: startTime
  type: string
- description: The end time of the time block
  name: endTime
  type: string
- description: The total hours recorded in the time block
  name: totalHours
  type: number
- description: The time code classification (Regular, Overtime, etc.)
  name: timeCode
  type: object
- description: The time zone for the time block
  name: timeZone
  type: string
- description: Optional comment for the time block
  name: comment
  type: string
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-time-block-schema.json
slug: workday-integration-time-block
source_filename: workday-integration-time-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/timeBlock\",\n  \"title\": \"Time Block\",\n  \"description\": \"Represents a time block recording worked hours for a worker within the Workday Time Tracking system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the time block\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the time block\"\n    },\n    \"worker\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker who recorded the time\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of the time block\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start time of the time\
  \ block\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The end time of the time block\"\n    },\n    \"totalHours\": {\n      \"type\": \"number\",\n      \"description\": \"The total hours recorded in the time block\"\n    },\n    \"timeCode\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The time code classification (Regular, Overtime, etc.)\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone for the time block\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment for the time block\"\n    }\n  },\n  \"required\": [\"id\", \"worker\", \"date\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n        \"href\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-time-block-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Time Block
---

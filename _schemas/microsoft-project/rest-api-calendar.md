---
description: Calendar schema from Microsoft Project Online REST API
layout: schema
name: Calendar
properties_list:
- description: Calendar identifier
  name: Id
  type: string
- description: Calendar name
  name: Name
  type: string
- description: Whether this is the standard calendar
  name: IsStandardCalendar
  type: boolean
- description: Calendar creation date
  name: Created
  type: string
- description: Calendar last modified date
  name: Modified
  type: string
provider_name: Microsoft Project
provider_slug: microsoft-project
schema_file: json-schema/rest-api-calendar-schema.json
slug: rest-api-calendar
source_filename: rest-api-calendar-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-calendar-schema.json\",\n  \"title\": \"Calendar\",\n  \"description\": \"Calendar schema from Microsoft Project Online REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Calendar identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Calendar name\"\n    },\n    \"IsStandardCalendar\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the standard calendar\"\n    },\n    \"Created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Calendar creation date\"\n    },\n    \"Modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Calendar last\
  \ modified date\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-calendar-schema.json
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio Management
- Project Management
- Resource Management
- Scheduling
- Task Management
title: Calendar
---

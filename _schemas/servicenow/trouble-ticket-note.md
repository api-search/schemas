---
description: ''
layout: schema
name: Note
properties_list:
- description: The type of note (always 'comments' in responses)
  name: '@type'
  type: string
- description: The comment text
  name: text
  type: string
- description: The date the comment was created
  name: date
  type: string
- description: The name of the user who wrote the comment
  name: author
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/trouble-ticket-note-schema.json
slug: trouble-ticket-note
source_filename: trouble-ticket-note-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of note (always 'comments' in responses)\",\n      \"example\": \"example_value\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The comment text\",\n      \"example\": \"example_value\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The date the comment was created\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user who wrote the comment\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Note\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-note-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: Note
---

---
description: ''
layout: schema
name: NoteInput
properties_list:
- description: Note text
  name: text
  type: string
- description: Type of note (determines whether recorded in Work notes or Additional comments field)
  name: '@type'
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/trouble-ticket-note-input-schema.json
slug: trouble-ticket-note-input
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Note text\",\n      \"example\": \"example_value\"\n    },\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of note (determines whether recorded in Work notes or Additional comments field)\",\n      \"example\": \"comments\",\n      \"enum\": [\n        \"comments\",\n        \"work_notes\"\n      ]\n    }\n  },\n  \"required\": [\n    \"text\",\n    \"@type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NoteInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-note-input-schema.json
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
title: NoteInput
---

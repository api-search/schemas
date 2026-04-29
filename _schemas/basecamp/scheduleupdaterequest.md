---
description: ''
layout: schema
name: ScheduleUpdateRequest
properties_list:
- description: Whether the schedule should include due dates from to-dos, cards, and steps
  name: include_due_assignments
  type: boolean
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/scheduleupdaterequest-schema.json
slug: scheduleupdaterequest
source_filename: scheduleupdaterequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/scheduleupdaterequest-schema.json\",\n  \"title\": \"ScheduleUpdateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"include_due_assignments\"\n  ],\n  \"properties\": {\n    \"include_due_assignments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the schedule should include due dates from to-dos, cards, and steps\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/scheduleupdaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ScheduleUpdateRequest
---

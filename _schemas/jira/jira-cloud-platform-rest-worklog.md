---
description: A worklog entry.
layout: schema
name: Worklog
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: ''
  name: started
  type: string
- description: The time spent on the worklog (e.g., 3h 20m).
  name: timeSpent
  type: string
- description: ''
  name: timeSpentSeconds
  type: integer
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-worklog-schema.json
slug: jira-cloud-platform-rest-worklog
source_filename: jira-cloud-platform-rest-worklog-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Worklog\",\n  \"type\": \"object\",\n  \"description\": \"A worklog entry.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"string\"\n    },\n    \"updated\": {\n      \"type\": \"string\"\n    },\n    \"started\": {\n      \"type\": \"string\"\n    },\n    \"timeSpent\": {\n      \"type\": \"string\",\n      \"description\": \"The time spent on the worklog (e.g., 3h 20m).\"\n    },\n    \"timeSpentSeconds\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-worklog-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Worklog
---

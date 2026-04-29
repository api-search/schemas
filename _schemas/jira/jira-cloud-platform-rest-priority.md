---
description: An issue priority.
layout: schema
name: Priority
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: string
- description: The name of the priority (e.g., Highest, High, Medium, Low, Lowest).
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: iconUrl
  type: string
- description: The color associated with the priority.
  name: statusColor
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-priority-schema.json
slug: jira-cloud-platform-rest-priority
source_filename: jira-cloud-platform-rest-priority-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Priority\",\n  \"type\": \"object\",\n  \"description\": \"An issue priority.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the priority (e.g., Highest, High, Medium, Low, Lowest).\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"iconUrl\": {\n      \"type\": \"string\"\n    },\n    \"statusColor\": {\n      \"type\": \"string\",\n      \"description\": \"The color associated with the priority.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-priority-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Priority
---

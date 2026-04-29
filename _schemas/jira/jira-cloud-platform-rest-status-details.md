---
description: A status in Jira.
layout: schema
name: StatusDetails
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: string
- description: The name of the status (e.g., To Do, In Progress, Done).
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: iconUrl
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-status-details-schema.json
slug: jira-cloud-platform-rest-status-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatusDetails\",\n  \"type\": \"object\",\n  \"description\": \"A status in Jira.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the status (e.g., To Do, In Progress, Done).\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"iconUrl\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-status-details-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: StatusDetails
---

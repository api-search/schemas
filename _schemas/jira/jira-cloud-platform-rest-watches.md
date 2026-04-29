---
description: The watchers of an issue.
layout: schema
name: Watches
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: watchCount
  type: integer
- description: ''
  name: isWatching
  type: boolean
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-watches-schema.json
slug: jira-cloud-platform-rest-watches
source_filename: jira-cloud-platform-rest-watches-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Watches\",\n  \"type\": \"object\",\n  \"description\": \"The watchers of an issue.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"watchCount\": {\n      \"type\": \"integer\"\n    },\n    \"isWatching\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-watches-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Watches
---

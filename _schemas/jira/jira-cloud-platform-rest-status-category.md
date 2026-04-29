---
description: A status category in Jira.
layout: schema
name: StatusCategory
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: integer
- description: The key of the status category (e.g., new, indeterminate, done).
  name: key
  type: string
- description: The color name for the status category.
  name: colorName
  type: string
- description: The name of the status category.
  name: name
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-status-category-schema.json
slug: jira-cloud-platform-rest-status-category
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatusCategory\",\n  \"type\": \"object\",\n  \"description\": \"A status category in Jira.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the status category (e.g., new, indeterminate, done).\"\n    },\n    \"colorName\": {\n      \"type\": \"string\",\n      \"description\": \"The color name for the status category.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the status category.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-status-category-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: StatusCategory
---

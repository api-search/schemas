---
description: A changelog entry.
layout: schema
name: ChangeHistory
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: items
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-change-history-schema.json
slug: jira-cloud-platform-rest-change-history
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChangeHistory\",\n  \"type\": \"object\",\n  \"description\": \"A changelog entry.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"string\"\n    },\n    \"items\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-change-history-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: ChangeHistory
---

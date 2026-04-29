---
description: Available transitions for an issue.
layout: schema
name: Transitions
properties_list:
- description: ''
  name: expand
  type: string
- description: ''
  name: transitions
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-transitions-schema.json
slug: jira-cloud-platform-rest-transitions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Transitions\",\n  \"type\": \"object\",\n  \"description\": \"Available transitions for an issue.\",\n  \"properties\": {\n    \"expand\": {\n      \"type\": \"string\"\n    },\n    \"transitions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-transitions-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Transitions
---

---
description: Issue type with its valid statuses.
layout: schema
name: IssueTypeWithStatus
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: subtask
  type: boolean
- description: ''
  name: statuses
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-issue-type-with-status-schema.json
slug: jira-cloud-platform-rest-issue-type-with-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssueTypeWithStatus\",\n  \"type\": \"object\",\n  \"description\": \"Issue type with its valid statuses.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"subtask\": {\n      \"type\": \"boolean\"\n    },\n    \"statuses\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-issue-type-with-status-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: IssueTypeWithStatus
---

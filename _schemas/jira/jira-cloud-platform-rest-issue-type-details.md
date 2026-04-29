---
description: Details of an issue type.
layout: schema
name: IssueTypeDetails
properties_list:
- description: The URL of the issue type in the REST API.
  name: self
  type: string
- description: The ID of the issue type.
  name: id
  type: string
- description: The description of the issue type.
  name: description
  type: string
- description: The URL of the issue type icon.
  name: iconUrl
  type: string
- description: The name of the issue type (e.g., Bug, Story, Task, Epic).
  name: name
  type: string
- description: Whether this issue type is used to create sub-tasks.
  name: subtask
  type: boolean
- description: The ID of the avatar for the issue type.
  name: avatarId
  type: integer
- description: The hierarchy level of the issue type.
  name: hierarchyLevel
  type: integer
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-issue-type-details-schema.json
slug: jira-cloud-platform-rest-issue-type-details
source_filename: jira-cloud-platform-rest-issue-type-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssueTypeDetails\",\n  \"type\": \"object\",\n  \"description\": \"Details of an issue type.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the issue type in the REST API.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the issue type.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the issue type.\"\n    },\n    \"iconUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the issue type icon.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the issue type (e.g., Bug, Story, Task, Epic).\"\n    },\n    \"subtask\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this issue type is used to create sub-tasks.\"\n    },\n    \"avatarId\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"The ID of the avatar for the issue type.\"\n    },\n    \"hierarchyLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"The hierarchy level of the issue type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-issue-type-details-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: IssueTypeDetails
---

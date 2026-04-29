---
description: Details of a newly created issue.
layout: schema
name: CreatedIssue
properties_list:
- description: The ID of the created issue.
  name: id
  type: string
- description: The key of the created issue (e.g., PROJ-123).
  name: key
  type: string
- description: The URL of the created issue in the REST API.
  name: self
  type: string
- description: Status of the transition applied during creation.
  name: transition
  type: object
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-created-issue-schema.json
slug: jira-cloud-platform-rest-created-issue
source_filename: jira-cloud-platform-rest-created-issue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreatedIssue\",\n  \"type\": \"object\",\n  \"description\": \"Details of a newly created issue.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the created issue.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the created issue (e.g., PROJ-123).\"\n    },\n    \"self\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the created issue in the REST API.\"\n    },\n    \"transition\": {\n      \"type\": \"object\",\n      \"description\": \"Status of the transition applied during creation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-created-issue-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: CreatedIssue
---

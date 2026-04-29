---
description: A comment on an issue.
layout: schema
name: Comment
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: string
- description: The rendered version of the comment body in HTML.
  name: renderedBody
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: Whether the comment is visible in Jira Service Management.
  name: jsdPublic
  type: boolean
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-comment-schema.json
slug: jira-cloud-platform-rest-comment
source_filename: jira-cloud-platform-rest-comment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Comment\",\n  \"type\": \"object\",\n  \"description\": \"A comment on an issue.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"renderedBody\": {\n      \"type\": \"string\",\n      \"description\": \"The rendered version of the comment body in HTML.\"\n    },\n    \"created\": {\n      \"type\": \"string\"\n    },\n    \"updated\": {\n      \"type\": \"string\"\n    },\n    \"jsdPublic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the comment is visible in Jira Service Management.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-comment-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Comment
---

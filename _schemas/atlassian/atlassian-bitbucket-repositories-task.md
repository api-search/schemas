---
description: A task object.
layout: schema
name: task
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: created_on
  type: string
- description: ''
  name: updated_on
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: content
  type: object
- description: ''
  name: pending
  type: boolean
- description: The ISO8601 timestamp for when the task was resolved.
  name: resolved_on
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-task-schema.json
slug: atlassian-bitbucket-repositories-task
source_filename: atlassian-bitbucket-repositories-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"task\",\n  \"type\": \"object\",\n  \"description\": \"A task object.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"created_on\": {\n      \"type\": \"string\"\n    },\n    \"updated_on\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"content\": {\n      \"type\": \"object\"\n    },\n    \"pending\": {\n      \"type\": \"boolean\"\n    },\n    \"resolved_on\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO8601 timestamp for when the task was resolved.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-task-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: task
---

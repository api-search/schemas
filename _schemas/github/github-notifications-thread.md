---
description: Thread
layout: schema
name: thread
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: repository
  type: object
- description: ''
  name: subject
  type: object
- description: ''
  name: reason
  type: string
- description: ''
  name: unread
  type: boolean
- description: ''
  name: updated_at
  type: string
- description: ''
  name: last_read_at
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: subscription_url
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-notifications-thread-schema.json
slug: github-notifications-thread
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-notifications-thread-schema.json\",\n  \"title\": \"thread\",\n  \"description\": \"Thread\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"12345678\"\n    },\n    \"repository\": {\n      \"$ref\": \"#/components/schemas/minimal-repository\"\n    },\n    \"subject\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\"\n        },\n        \"url\": {\n          \"type\": \"string\"\n        },\n        \"latest_comment_url\": {\n          \"type\": \"string\"\n        },\n        \"type\": {\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\n        \"title\",\n        \"url\",\n        \"latest_comment_url\",\n        \"type\"\n      ]\n    },\n    \"reason\"\
  : {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"unread\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"last_read_at\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"subscription_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/notifications/threads/2/subscription\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"unread\",\n    \"reason\",\n    \"updated_at\",\n    \"last_read_at\",\n    \"subject\",\n    \"repository\",\n    \"url\",\n    \"subscription_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-notifications-thread-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: thread
---

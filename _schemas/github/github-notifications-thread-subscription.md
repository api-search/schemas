---
description: Thread Subscription
layout: schema
name: thread-subscription
properties_list:
- description: ''
  name: subscribed
  type: boolean
- description: ''
  name: ignored
  type: boolean
- description: ''
  name: reason
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: thread_url
  type: string
- description: ''
  name: repository_url
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-notifications-thread-subscription-schema.json
slug: github-notifications-thread-subscription
source_filename: github-notifications-thread-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-notifications-thread-subscription-schema.json\",\n  \"title\": \"thread-subscription\",\n  \"description\": \"Thread Subscription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscribed\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"ignored\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"example_value\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2012-10-06T21:34:12Z\",\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/notifications/threads/1/subscription\"\n    },\n    \"thread_url\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/notifications/threads/1\"\n    },\n    \"repository_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/1\"\n    }\n  },\n  \"required\": [\n    \"created_at\",\n    \"ignored\",\n    \"reason\",\n    \"url\",\n    \"subscribed\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-notifications-thread-subscription-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: thread-subscription
---

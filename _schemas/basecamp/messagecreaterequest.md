---
description: ''
layout: schema
name: MessageCreateRequest
properties_list:
- description: Message subject (title)
  name: subject
  type: string
- description: Message body in HTML format
  name: content
  type: string
- description: Set to "active" to publish immediately
  name: status
  type: string
- description: Optional message category ID
  name: category_id
  type: integer
- description: Person IDs to notify about this message
  name: subscriptions
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/messagecreaterequest-schema.json
slug: messagecreaterequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/messagecreaterequest-schema.json\",\n  \"title\": \"MessageCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"subject\"\n  ],\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Message subject (title)\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Message body in HTML format\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Set to \\\"active\\\" to publish immediately\",\n      \"enum\": [\n        \"active\",\n        \"draft\"\n      ]\n    },\n    \"category_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Optional message category ID\"\n    },\n    \"subscriptions\": {\n      \"type\": \"array\",\n      \"description\": \"Person IDs to notify about this message\",\n      \"items\": {\n    \
  \    \"type\": \"integer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/messagecreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: MessageCreateRequest
---

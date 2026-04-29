---
description: ''
layout: schema
name: Message
properties_list:
- description: Message identifier
  name: messageId
  type: string
- description: Correlation identifier
  name: correlationId
  type: string
- description: Time the message was put
  name: putDateTime
  type: string
- description: ''
  name: persistence
  type: string
- description: Reply-to queue name
  name: replyToQueue
  type: string
- description: Reply-to queue manager name
  name: replyToQueueManager
  type: string
- description: Message expiry in tenths of a second
  name: expiry
  type: integer
- description: Message body content
  name: body
  type: string
- description: Message format
  name: format
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-mq-rest-message-schema.json
slug: websphere-mq-rest-message
source_filename: websphere-mq-rest-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Message\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"Message identifier\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation identifier\"\n    },\n    \"putDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time the message was put\"\n    },\n    \"persistence\": {\n      \"type\": \"string\"\n    },\n    \"replyToQueue\": {\n      \"type\": \"string\",\n      \"description\": \"Reply-to queue name\"\n    },\n    \"replyToQueueManager\": {\n      \"type\": \"string\",\n      \"description\": \"Reply-to queue manager name\"\n    },\n    \"expiry\": {\n      \"type\": \"integer\",\n      \"description\": \"Message expiry in tenths of a second\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Message body content\"\n\
  \    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Message format\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-mq-rest-message-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Message
---

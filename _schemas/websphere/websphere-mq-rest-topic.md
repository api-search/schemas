---
description: ''
layout: schema
name: Topic
properties_list:
- description: Administrative topic object name
  name: name
  type: string
- description: Topic string
  name: topicString
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: durableSubscriptions
  type: string
- description: ''
  name: publish
  type: string
- description: ''
  name: subscribe
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-mq-rest-topic-schema.json
slug: websphere-mq-rest-topic
source_filename: websphere-mq-rest-topic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Topic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative topic object name\"\n    },\n    \"topicString\": {\n      \"type\": \"string\",\n      \"description\": \"Topic string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"durableSubscriptions\": {\n      \"type\": \"string\"\n    },\n    \"publish\": {\n      \"type\": \"string\"\n    },\n    \"subscribe\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-mq-rest-topic-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Topic
---

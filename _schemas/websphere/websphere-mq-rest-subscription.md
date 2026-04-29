---
description: ''
layout: schema
name: Subscription
properties_list:
- description: Subscription identifier
  name: id
  type: string
- description: Subscription name
  name: name
  type: string
- description: Topic string
  name: topicString
  type: string
- description: Destination queue name
  name: destination
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: durability
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-mq-rest-subscription-schema.json
slug: websphere-mq-rest-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription name\"\n    },\n    \"topicString\": {\n      \"type\": \"string\",\n      \"description\": \"Topic string\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination queue name\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"durability\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-mq-rest-subscription-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Subscription
---

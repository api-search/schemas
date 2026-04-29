---
description: ''
layout: schema
name: NotificationSubscription
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: objectName
  type: string
- description: ''
  name: filters
  type: array
- description: ''
  name: created
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-rest-connector-notification-subscription-schema.json
slug: websphere-liberty-rest-connector-notification-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationSubscription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"objectName\": {\n      \"type\": \"string\"\n    },\n    \"filters\": {\n      \"type\": \"array\"\n    },\n    \"created\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-rest-connector-notification-subscription-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: NotificationSubscription
---

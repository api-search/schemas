---
description: NotificationEventTopicRoute schema from Ampersand API
layout: schema
name: NotificationEventTopicRoute
properties_list:
- description: The event-topic route ID.
  name: id
  type: string
- description: ''
  name: eventType
  type: object
- description: The ID of the topic to route events to.
  name: topicId
  type: string
- description: The Ampersand project ID.
  name: projectId
  type: string
- description: The time when the event-topic route was created.
  name: createTime
  type: string
- description: The time when the event-topic route was last updated.
  name: updateTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-notification-event-topic-route-schema.json
slug: ampersand-api-notification-event-topic-route
source_filename: ampersand-api-notification-event-topic-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-notification-event-topic-route-schema.json\",\n  \"title\": \"NotificationEventTopicRoute\",\n  \"description\": \"NotificationEventTopicRoute schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The event-topic route ID.\"\n    },\n    \"eventType\": {\n      \"$ref\": \"#/components/schemas/NotificationEventType\"\n    },\n    \"topicId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the topic to route events to.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The Ampersand project ID.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the event-topic route was\
  \ created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the event-topic route was last updated.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"eventType\",\n    \"topicId\",\n    \"projectId\",\n    \"createTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-notification-event-topic-route-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: NotificationEventTopicRoute
---

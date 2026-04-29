---
description: An event in the Boltic Streams real-time event streaming system, representing a tracked action from a website, mobile app, or server.
layout: schema
name: Boltic Stream Event
properties_list:
- description: Unique identifier for the event
  name: id
  type: string
- description: ID of the stream source that received the event
  name: sourceId
  type: string
- description: Event type name (e.g., page_view, purchase, signup)
  name: type
  type: string
- description: Custom event properties
  name: properties
  type: object
- description: Contextual information about the event
  name: context
  type: object
- description: Identified user ID
  name: userId
  type: string
- description: Anonymous user identifier
  name: anonymousId
  type: string
- description: Client-side timestamp of when the event occurred
  name: timestamp
  type: string
- description: Server-side timestamp of when the event was received
  name: receivedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-stream-event.json
slug: boltic-stream-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-stream-event.json\",\n  \"title\": \"Boltic Stream Event\",\n  \"description\": \"An event in the Boltic Streams real-time event streaming system, representing a tracked action from a website, mobile app, or server.\",\n  \"type\": \"object\",\n  \"required\": [\"sourceId\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the event\"\n    },\n    \"sourceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the stream source that received the event\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Event type name (e.g., page_view, purchase, signup)\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Custom event\
  \ properties\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ip\": {\n          \"type\": \"string\",\n          \"format\": \"ipv4\"\n        },\n        \"userAgent\": {\n          \"type\": \"string\"\n        },\n        \"locale\": {\n          \"type\": \"string\"\n        },\n        \"page\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            },\n            \"title\": {\n              \"type\": \"string\"\n            },\n            \"referrer\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      },\n      \"description\": \"Contextual information about the event\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Identified user ID\"\n    },\n    \"anonymousId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Anonymous user identifier\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Client-side timestamp of when the event occurred\"\n    },\n    \"receivedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Server-side timestamp of when the event was received\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-stream-event.json
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Stream Event
---

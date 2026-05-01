---
description: An event within a conversation, representing a message, reply, reaction, edit, deletion, file transfer, or participant action in the Global Relay Archive.
layout: schema
name: Global Relay Event
properties_list:
- description: Type of conversation event
  name: eventType
  type: string
- description: Timestamp of the event in ISO 8601 format
  name: timestamp
  type: string
- description: The participant who triggered this event
  name: sender
  type: object
- description: Content body of the event
  name: body
  type: string
- description: IDs of files uploaded via /files endpoint
  name: fileIds
  type: array
- description: ID of the event being replied to, edited, or deleted
  name: referencedEventId
  type: string
provider_name: Global Relay
provider_slug: global-relay
schema_file: json-schema/global-relay-event.json
slug: global-relay-event
source_filename: global-relay-event.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"global-relay-event.json\",\n  \"title\": \"Global Relay Event\",\n  \"description\": \"An event within a conversation, representing a message, reply, reaction, edit, deletion, file transfer, or participant action in the Global Relay Archive.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"eventType\",\n    \"timestamp\"\n  ],\n  \"properties\": {\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of conversation event\",\n      \"enum\": [\n        \"Message\",\n        \"Reply\",\n        \"Reaction\",\n        \"Edit\",\n        \"Delete\",\n        \"File_transfer\",\n        \"Participant_join\",\n        \"Participant_leave\",\n        \"Call_start\",\n        \"Call_end\"\n      ]\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the event in ISO 8601 format\"\n    },\n\
  \    \"sender\": {\n      \"$ref\": \"global-relay-participant.json\",\n      \"description\": \"The participant who triggered this event\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Content body of the event\"\n    },\n    \"fileIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of files uploaded via /files endpoint\"\n    },\n    \"referencedEventId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the event being replied to, edited, or deleted\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/json-schema/global-relay-event.json
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
title: Global Relay Event
---

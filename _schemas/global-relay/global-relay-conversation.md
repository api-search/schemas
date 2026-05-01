---
description: A conversation archived in the Global Relay Archive, representing a one-to-one or multi-party messaging exchange including messages, reactions, edits, and file transfers.
layout: schema
name: Global Relay Conversation
properties_list:
- description: Unique identifier for the conversation
  name: conversationId
  type: string
- description: The type of messaging channel
  name: channelType
  type: string
- description: Title or subject of the conversation
  name: title
  type: string
- description: List of participants in the conversation
  name: participants
  type: array
- description: List of events in the conversation
  name: events
  type: array
provider_name: Global Relay
provider_slug: global-relay
schema_file: json-schema/global-relay-conversation.json
slug: global-relay-conversation
source_filename: global-relay-conversation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"global-relay-conversation.json\",\n  \"title\": \"Global Relay Conversation\",\n  \"description\": \"A conversation archived in the Global Relay Archive, representing a one-to-one or multi-party messaging exchange including messages, reactions, edits, and file transfers.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"conversationId\",\n    \"channelType\",\n    \"events\"\n  ],\n  \"properties\": {\n    \"conversationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the conversation\"\n    },\n    \"channelType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of messaging channel\",\n      \"enum\": [\n        \"IM\",\n        \"GroupChat\",\n        \"Channel\",\n        \"SMS\",\n        \"MMS\",\n        \"Other\"\n      ]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title or subject of the conversation\"\
  \n    },\n    \"participants\": {\n      \"type\": \"array\",\n      \"description\": \"List of participants in the conversation\",\n      \"items\": {\n        \"$ref\": \"global-relay-participant.json\"\n      }\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"List of events in the conversation\",\n      \"items\": {\n        \"$ref\": \"global-relay-event.json\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/json-schema/global-relay-conversation.json
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
title: Global Relay Conversation
---

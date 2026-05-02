---
description: Schema for the MassTransit message envelope format. All messages sent through MassTransit are wrapped in this envelope containing routing, correlation, and metadata information.
layout: schema
name: MassTransit Message Envelope
properties_list:
- description: Unique identifier for the message
  name: messageId
  type: string
- description: Request identifier for request/response conversations
  name: requestId
  type: string
- description: Correlation identifier for tracking related messages
  name: correlationId
  type: string
- description: Conversation identifier (created on first message, propagated through chain)
  name: conversationId
  type: string
- description: The messageId of the message that initiated this message
  name: initiatorId
  type: string
- description: The address of the endpoint that sent the message
  name: sourceAddress
  type: string
- description: The destination endpoint address
  name: destinationAddress
  type: string
- description: The address for response messages
  name: responseAddress
  type: string
- description: The address for fault messages
  name: faultAddress
  type: string
- description: URN-formatted message type identifiers, e.g., urn:message:Namespace:MessageType
  name: messageType
  type: array
- description: The actual message payload
  name: message
  type: object
- description: Time at which the message expires
  name: expirationTime
  type: string
- description: Time when the message was sent
  name: sentTime
  type: string
- description: Custom headers as key-value pairs
  name: headers
  type: object
- description: Information about the host that sent the message
  name: host
  type: object
provider_name: MassTransit
provider_slug: masstransit
schema_file: json-schema/masstransit-message-envelope.json
slug: masstransit-message-envelope
source_filename: masstransit-message-envelope.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/masstransit/masstransit-message-envelope.json\",\n  \"title\": \"MassTransit Message Envelope\",\n  \"description\": \"Schema for the MassTransit message envelope format. All messages sent through MassTransit are wrapped in this envelope containing routing, correlation, and metadata information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messageId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the message\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Request identifier for request/response conversations\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Correlation identifier for tracking related messages\"\n    },\n    \"conversationId\": {\n   \
  \   \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Conversation identifier (created on first message, propagated through chain)\"\n    },\n    \"initiatorId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The messageId of the message that initiated this message\"\n    },\n    \"sourceAddress\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The address of the endpoint that sent the message\"\n    },\n    \"destinationAddress\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The destination endpoint address\"\n    },\n    \"responseAddress\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The address for response messages\"\n    },\n    \"faultAddress\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The address for fault messages\"\n    },\n    \"messageType\": {\n \
  \     \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"URN-formatted message type identifiers, e.g., urn:message:Namespace:MessageType\"\n    },\n    \"message\": {\n      \"type\": \"object\",\n      \"description\": \"The actual message payload\"\n    },\n    \"expirationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time at which the message expires\"\n    },\n    \"sentTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time when the message was sent\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Custom headers as key-value pairs\"\n    },\n    \"host\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the host that sent the message\",\n      \"properties\": {\n        \"machineName\": {\n          \"type\": \"string\"\n     \
  \   },\n        \"processName\": {\n          \"type\": \"string\"\n        },\n        \"processId\": {\n          \"type\": \"integer\"\n        },\n        \"assembly\": {\n          \"type\": \"string\"\n        },\n        \"assemblyVersion\": {\n          \"type\": \"string\"\n        },\n        \"frameworkVersion\": {\n          \"type\": \"string\"\n        },\n        \"massTransitVersion\": {\n          \"type\": \"string\"\n        },\n        \"operatingSystemVersion\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"messageId\", \"messageType\", \"message\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/masstransit/refs/heads/main/json-schema/masstransit-message-envelope.json
tags:
- .NET
- Event-Driven
- Message Bus
- Messaging
- Open Source
- Sagas
title: MassTransit Message Envelope
---

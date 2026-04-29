---
description: Schema describing the standard AMQP 0-9-1 message properties (Basic.Properties). These properties are defined in the AMQP specification and provide metadata about the message content, delivery, and routing.
layout: schema
name: AMQP Message Properties
properties_list:
- description: MIME content type of the message body (e.g., application/json, text/plain).
  name: contentType
  type: string
- description: MIME content encoding of the message body (e.g., utf-8, gzip).
  name: contentEncoding
  type: string
- description: Application-specific message headers as an AMQP field table.
  name: headers
  type: object
- description: Message delivery mode. 1 = non-persistent (may be lost on broker restart), 2 = persistent (written to disk).
  name: deliveryMode
  type: integer
- description: Message priority level from 0 (lowest) to 9 (highest).
  name: priority
  type: integer
- description: Application-defined correlation identifier, typically used to correlate RPC responses with requests.
  name: correlationId
  type: string
- description: Name of the queue to which replies should be sent, used in the request/reply messaging pattern.
  name: replyTo
  type: string
- description: Message expiration (TTL) as a string representing milliseconds. The message will be discarded after this duration.
  name: expiration
  type: string
- description: Application-defined unique message identifier.
  name: messageId
  type: string
- description: Message timestamp as a UNIX epoch timestamp (seconds since 1970-01-01T00:00:00Z).
  name: timestamp
  type: integer
- description: Application-defined message type name, used to describe the kind of message.
  name: type
  type: string
- description: The user ID of the authenticated user who published the message. Validated by the broker against the connection credentials.
  name: userId
  type: string
- description: Application identifier of the publishing application.
  name: appId
  type: string
- description: Cluster identifier for use by clustering applications. Deprecated in AMQP 0-9-1.
  name: clusterId
  type: string
provider_name: AMQP
provider_slug: amqp
schema_file: json-schema/amqp-message-properties.json
slug: amqp-message-properties
source_json: "{\n  \"$id\": \"amqp-message-properties.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AMQP Message Properties\",\n  \"description\": \"Schema describing the standard AMQP 0-9-1 message properties (Basic.Properties). These properties are defined in the AMQP specification and provide metadata about the message content, delivery, and routing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME content type of the message body (e.g., application/json, text/plain).\",\n      \"examples\": [\n        \"application/json\",\n        \"text/plain\",\n        \"application/octet-stream\"\n      ]\n    },\n    \"contentEncoding\": {\n      \"type\": \"string\",\n      \"description\": \"MIME content encoding of the message body (e.g., utf-8, gzip).\",\n      \"examples\": [\n        \"utf-8\",\n        \"gzip\"\n      ]\n    },\n    \"headers\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Application-specific message headers as an AMQP field table.\",\n      \"additionalProperties\": true\n    },\n    \"deliveryMode\": {\n      \"type\": \"integer\",\n      \"description\": \"Message delivery mode. 1 = non-persistent (may be lost on broker restart), 2 = persistent (written to disk).\",\n      \"enum\": [1, 2]\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Message priority level from 0 (lowest) to 9 (highest).\",\n      \"minimum\": 0,\n      \"maximum\": 9\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Application-defined correlation identifier, typically used to correlate RPC responses with requests.\",\n      \"format\": \"uuid\"\n    },\n    \"replyTo\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the queue to which replies should be sent, used in the request/reply messaging pattern.\"\n    },\n    \"expiration\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Message expiration (TTL) as a string representing milliseconds. The message will be discarded after this duration.\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"Application-defined unique message identifier.\",\n      \"format\": \"uuid\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Message timestamp as a UNIX epoch timestamp (seconds since 1970-01-01T00:00:00Z).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Application-defined message type name, used to describe the kind of message.\",\n      \"examples\": [\n        \"order.created\",\n        \"payment.processed\",\n        \"user.registered\"\n      ]\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the authenticated user who published the message. Validated by the broker against the connection credentials.\"\
  \n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Application identifier of the publishing application.\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster identifier for use by clustering applications. Deprecated in AMQP 0-9-1.\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amqp/refs/heads/main/json-schema/amqp-message-properties.json
tags:
- AMQP
- Asynchronous
- Message Queue
- Messaging
- Middleware
- Open Standard
- Publish Subscribe
title: AMQP Message Properties
---

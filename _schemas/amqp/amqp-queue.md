---
description: Schema describing an AMQP 0-9-1 queue. Queues store messages and deliver them to consumers. They can be durable, exclusive, or auto-deleted, and support various arguments for controlling message TTL, length limits, and dead-lettering.
layout: schema
name: AMQP Queue
properties_list:
- description: The name of the queue. An empty string causes the broker to generate a unique name.
  name: name
  type: string
- description: If true, the queue survives broker restarts.
  name: durable
  type: boolean
- description: If true, the queue is used by only one connection and will be deleted when that connection closes.
  name: exclusive
  type: boolean
- description: If true, the queue is automatically deleted when the last consumer unsubscribes.
  name: autoDelete
  type: boolean
- description: Optional arguments for queue declaration providing extended configuration.
  name: arguments
  type: object
provider_name: AMQP
provider_slug: amqp
schema_file: json-schema/amqp-queue.json
slug: amqp-queue
source_filename: amqp-queue.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"amqp-queue.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AMQP Queue\",\n  \"description\": \"Schema describing an AMQP 0-9-1 queue. Queues store messages and deliver them to consumers. They can be durable, exclusive, or auto-deleted, and support various arguments for controlling message TTL, length limits, and dead-lettering.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the queue. An empty string causes the broker to generate a unique name.\"\n    },\n    \"durable\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the queue survives broker restarts.\",\n      \"default\": false\n    },\n    \"exclusive\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the queue is used by only one connection and will be deleted when that connection closes.\",\n      \"\
  default\": false\n    },\n    \"autoDelete\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the queue is automatically deleted when the last consumer unsubscribes.\",\n      \"default\": false\n    },\n    \"arguments\": {\n      \"type\": \"object\",\n      \"description\": \"Optional arguments for queue declaration providing extended configuration.\",\n      \"properties\": {\n        \"x-message-ttl\": {\n          \"type\": \"integer\",\n          \"description\": \"Per-queue message time-to-live in milliseconds. Messages older than this are discarded or dead-lettered.\",\n          \"minimum\": 0\n        },\n        \"x-expires\": {\n          \"type\": \"integer\",\n          \"description\": \"Queue expiry time in milliseconds. The queue is deleted after being unused for this duration.\",\n          \"minimum\": 0\n        },\n        \"x-max-length\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of messages the queue can\
  \ hold. Overflow behavior is controlled by x-overflow.\",\n          \"minimum\": 0\n        },\n        \"x-max-length-bytes\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum total size in bytes of all messages in the queue.\",\n          \"minimum\": 0\n        },\n        \"x-overflow\": {\n          \"type\": \"string\",\n          \"description\": \"Overflow behavior when x-max-length or x-max-length-bytes is reached.\",\n          \"enum\": [\n            \"drop-head\",\n            \"reject-publish\",\n            \"reject-publish-dlx\"\n          ]\n        },\n        \"x-dead-letter-exchange\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the exchange to which dead-lettered messages are republished.\"\n        },\n        \"x-dead-letter-routing-key\": {\n          \"type\": \"string\",\n          \"description\": \"Routing key to use when dead-lettering messages. If not set, the original routing key is used.\"\n        },\n\
  \        \"x-max-priority\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum priority level the queue supports (0-255). Enables priority queuing.\",\n          \"minimum\": 0,\n          \"maximum\": 255\n        },\n        \"x-queue-mode\": {\n          \"type\": \"string\",\n          \"description\": \"Queue mode. 'lazy' mode moves messages to disk as early as possible to reduce memory usage.\",\n          \"enum\": [\n            \"default\",\n            \"lazy\"\n          ]\n        },\n        \"x-queue-type\": {\n          \"type\": \"string\",\n          \"description\": \"The queue type. Classic queues are the default; quorum queues provide data safety via replication.\",\n          \"enum\": [\n            \"classic\",\n            \"quorum\",\n            \"stream\"\n          ]\n        }\n      },\n      \"additionalProperties\": true\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amqp/refs/heads/main/json-schema/amqp-queue.json
tags:
- AMQP
- Asynchronous
- Message Queue
- Messaging
- Middleware
- Open Standard
- Publish Subscribe
title: AMQP Queue
---

---
description: Schema for a RabbitMQ AMQP message including properties and payload.
layout: schema
name: RabbitMQ Message
properties_list:
- description: The message body content
  name: payload
  type: object
- description: Size of the payload in bytes
  name: payload_bytes
  type: integer
- description: The exchange the message was published to
  name: exchange
  type: string
- description: The routing key used for message routing
  name: routing_key
  type: string
- description: Whether the message has been redelivered
  name: redelivered
  type: boolean
- description: AMQP message properties
  name: properties
  type: object
provider_name: RabbitMQ
provider_slug: rabbitmq
schema_file: json-schema/rabbitmq-message.json
slug: rabbitmq-message
source_filename: rabbitmq-message.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/rabbitmq/rabbitmq-message.json\",\n  \"title\": \"RabbitMQ Message\",\n  \"description\": \"Schema for a RabbitMQ AMQP message including properties and payload.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"payload\": {\n      \"description\": \"The message body content\"\n    },\n    \"payload_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the payload in bytes\"\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"The exchange the message was published to\"\n    },\n    \"routing_key\": {\n      \"type\": \"string\",\n      \"description\": \"The routing key used for message routing\"\n    },\n    \"redelivered\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the message has been redelivered\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"AMQP message properties\",\n      \"properties\": {\n        \"content_type\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the message body\"\n        },\n        \"content_encoding\": {\n          \"type\": \"string\",\n          \"description\": \"Encoding of the message body\"\n        },\n        \"delivery_mode\": {\n          \"type\": \"integer\",\n          \"enum\": [1, 2],\n          \"description\": \"1=non-persistent, 2=persistent\"\n        },\n        \"priority\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 255,\n          \"description\": \"Message priority\"\n        },\n        \"correlation_id\": {\n          \"type\": \"string\",\n          \"description\": \"Correlation identifier for RPC patterns\"\n        },\n        \"reply_to\": {\n          \"type\": \"string\",\n          \"description\": \"Queue name for reply messages\"\n        },\n        \"expiration\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Per-message TTL in milliseconds\"\n        },\n        \"message_id\": {\n          \"type\": \"string\",\n          \"description\": \"Application-provided message identifier\"\n        },\n        \"timestamp\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix timestamp when message was created\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Application-specific message type\"\n        },\n        \"user_id\": {\n          \"type\": \"string\",\n          \"description\": \"User who published the message\"\n        },\n        \"app_id\": {\n          \"type\": \"string\",\n          \"description\": \"Application that published the message\"\n        },\n        \"headers\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Custom message headers\"\n        }\n      }\n    }\n  },\n  \"required\": [\"payload\"]\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/json-schema/rabbitmq-message.json
tags:
- AMQP
- Distributed Systems
- Event Streaming
- Message Broker
- Messaging
- Queue
title: RabbitMQ Message
---

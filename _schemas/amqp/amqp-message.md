---
description: Schema describing the structure of an AMQP 0-9-1 message including properties, headers, and payload. An AMQP message consists of message properties (metadata), application headers, and a binary payload body.
layout: schema
name: AMQP Message
properties_list:
- description: ''
  name: properties
  type: object
- description: Application-specific headers as key-value pairs sent in the message header frame.
  name: headers
  type: object
- description: The message body content. Can be any valid JSON value or a binary payload represented as a base64-encoded string.
  name: body
  type: object
- description: The exchange the message was published to.
  name: exchange
  type: string
- description: The routing key used when publishing the message.
  name: routingKey
  type: string
- description: If true, the server will return an undeliverable message with a Return method. If false, the server silently drops the message.
  name: mandatory
  type: boolean
- description: If true, the server will return an undeliverable message if it cannot be immediately consumed. Deprecated in AMQP 0-9-1.
  name: immediate
  type: boolean
provider_name: AMQP
provider_slug: amqp
schema_file: json-schema/amqp-message.json
slug: amqp-message
source_filename: amqp-message.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"amqp-message.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AMQP Message\",\n  \"description\": \"Schema describing the structure of an AMQP 0-9-1 message including properties, headers, and payload. An AMQP message consists of message properties (metadata), application headers, and a binary payload body.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"body\"\n  ],\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"amqp-message-properties.json\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Application-specific headers as key-value pairs sent in the message header frame.\",\n      \"additionalProperties\": true\n    },\n    \"body\": {\n      \"description\": \"The message body content. Can be any valid JSON value or a binary payload represented as a base64-encoded string.\",\n      \"oneOf\": [\n        {\n          \"type\": \"object\",\n          \"additionalProperties\"\
  : true\n        },\n        {\n          \"type\": \"array\"\n        },\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"boolean\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"The exchange the message was published to.\"\n    },\n    \"routingKey\": {\n      \"type\": \"string\",\n      \"description\": \"The routing key used when publishing the message.\"\n    },\n    \"mandatory\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the server will return an undeliverable message with a Return method. If false, the server silently drops the message.\",\n      \"default\": false\n    },\n    \"immediate\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the server will return an undeliverable message if it cannot be immediately consumed. Deprecated\
  \ in AMQP 0-9-1.\",\n      \"default\": false\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amqp/refs/heads/main/json-schema/amqp-message.json
tags:
- AMQP
- Asynchronous
- Message Queue
- Messaging
- Middleware
- Open Standard
- Publish Subscribe
title: AMQP Message
---

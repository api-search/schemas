---
description: Schema describing an AMQP 0-9-1 exchange. Exchanges receive messages from producers and route them to queues based on the exchange type and binding rules. The four standard exchange types are direct, topic, fanout, and headers.
layout: schema
name: AMQP Exchange
properties_list:
- description: The name of the exchange. The empty string denotes the default (nameless) direct exchange.
  name: name
  type: string
- description: The exchange type which determines the routing algorithm.
  name: type
  type: string
- description: If true, the exchange survives broker restarts. Non-durable exchanges are deleted on restart.
  name: durable
  type: boolean
- description: If true, the exchange is automatically deleted when the last queue is unbound from it.
  name: autoDelete
  type: boolean
- description: If true, the exchange cannot be directly published to by clients; it can only receive messages from other exchanges via exchange-to-exchange bindings.
  name: internal
  type: boolean
- description: Optional arguments for exchange declaration, used for broker-specific extensions (e.g., alternate exchange).
  name: arguments
  type: object
provider_name: AMQP
provider_slug: amqp
schema_file: json-schema/amqp-exchange.json
slug: amqp-exchange
source_json: "{\n  \"$id\": \"amqp-exchange.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AMQP Exchange\",\n  \"description\": \"Schema describing an AMQP 0-9-1 exchange. Exchanges receive messages from producers and route them to queues based on the exchange type and binding rules. The four standard exchange types are direct, topic, fanout, and headers.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"type\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the exchange. The empty string denotes the default (nameless) direct exchange.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The exchange type which determines the routing algorithm.\",\n      \"enum\": [\n        \"direct\",\n        \"topic\",\n        \"fanout\",\n        \"headers\"\n      ]\n    },\n    \"durable\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"If true, the exchange survives broker restarts. Non-durable exchanges are deleted on restart.\",\n      \"default\": false\n    },\n    \"autoDelete\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the exchange is automatically deleted when the last queue is unbound from it.\",\n      \"default\": false\n    },\n    \"internal\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the exchange cannot be directly published to by clients; it can only receive messages from other exchanges via exchange-to-exchange bindings.\",\n      \"default\": false\n    },\n    \"arguments\": {\n      \"type\": \"object\",\n      \"description\": \"Optional arguments for exchange declaration, used for broker-specific extensions (e.g., alternate exchange).\",\n      \"properties\": {\n        \"alternate-exchange\": {\n          \"type\": \"string\",\n          \"description\": \"Name of an alternate exchange to route messages to when they cannot be routed by this\
  \ exchange.\"\n        }\n      },\n      \"additionalProperties\": true\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amqp/refs/heads/main/json-schema/amqp-exchange.json
tags:
- AMQP
- Asynchronous
- Message Queue
- Messaging
- Middleware
- Open Standard
- Publish Subscribe
title: AMQP Exchange
---

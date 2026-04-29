---
description: Schema describing an AMQP 0-9-1 binding. Bindings are rules that exchanges use to route messages to queues. A binding links a queue to an exchange with a routing key and optional arguments for headers-based matching.
layout: schema
name: AMQP Binding
properties_list:
- description: The name of the exchange from which messages are routed.
  name: source
  type: string
- description: The name of the queue or exchange to which messages are routed.
  name: destination
  type: string
- description: Whether the destination is a queue or an exchange.
  name: destinationType
  type: string
- description: 'The routing key for the binding. For topic exchanges, supports wildcards: * matches one word, # matches zero or more words.'
  name: routingKey
  type: string
- description: Optional arguments for the binding. Used primarily with headers exchanges for matching on message header values.
  name: arguments
  type: object
provider_name: AMQP
provider_slug: amqp
schema_file: json-schema/amqp-binding.json
slug: amqp-binding
source_json: "{\n  \"$id\": \"amqp-binding.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AMQP Binding\",\n  \"description\": \"Schema describing an AMQP 0-9-1 binding. Bindings are rules that exchanges use to route messages to queues. A binding links a queue to an exchange with a routing key and optional arguments for headers-based matching.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"source\",\n    \"destination\"\n  ],\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the exchange from which messages are routed.\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the queue or exchange to which messages are routed.\"\n    },\n    \"destinationType\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the destination is a queue or an exchange.\",\n      \"enum\": [\n        \"queue\",\n        \"exchange\"\n      ],\n\
  \      \"default\": \"queue\"\n    },\n    \"routingKey\": {\n      \"type\": \"string\",\n      \"description\": \"The routing key for the binding. For topic exchanges, supports wildcards: * matches one word, # matches zero or more words.\",\n      \"examples\": [\n        \"orders.created\",\n        \"orders.*\",\n        \"orders.#\",\n        \"\"\n      ]\n    },\n    \"arguments\": {\n      \"type\": \"object\",\n      \"description\": \"Optional arguments for the binding. Used primarily with headers exchanges for matching on message header values.\",\n      \"properties\": {\n        \"x-match\": {\n          \"type\": \"string\",\n          \"description\": \"Matching algorithm for headers exchange bindings. 'all' requires all headers to match, 'any' requires at least one.\",\n          \"enum\": [\n            \"all\",\n            \"any\"\n          ]\n        }\n      },\n      \"additionalProperties\": true\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amqp/refs/heads/main/json-schema/amqp-binding.json
tags:
- AMQP
- Asynchronous
- Message Queue
- Messaging
- Middleware
- Open Standard
- Publish Subscribe
title: AMQP Binding
---

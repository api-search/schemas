---
description: A message to be placed in an actor's mailbox
layout: schema
name: ActorMessage
properties_list:
- description: Message type discriminator
  name: type
  type: string
- description: Message payload
  name: payload
  type: object
- description: Actor ID to send reply to (optional)
  name: replyTo
  type: string
- description: Correlation ID for tracing
  name: correlationId
  type: string
- description: Message priority in mailbox
  name: priority
  type: string
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-actor-message-schema.json
slug: actor-model-actor-message
source_filename: actor-model-actor-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-actormessage-schema.json\",\n  \"title\": \"ActorMessage\",\n  \"description\": \"A message to be placed in an actor's mailbox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Message type discriminator\",\n      \"example\": \"UpdateProfile\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Message payload\",\n      \"additionalProperties\": true\n    },\n    \"replyTo\": {\n      \"type\": \"string\",\n      \"description\": \"Actor ID to send reply to (optional)\",\n      \"example\": \"caller-actor-456\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation ID for tracing\",\n      \"example\": \"trace-xyz-789\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\n\
  \        \"high\",\n        \"normal\",\n        \"low\"\n      ],\n      \"description\": \"Message priority in mailbox\",\n      \"example\": \"normal\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-actor-message-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: ActorMessage
---

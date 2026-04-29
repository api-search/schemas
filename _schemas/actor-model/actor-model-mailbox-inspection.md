---
description: Inspection of pending messages in an actor's mailbox
layout: schema
name: MailboxInspection
properties_list:
- description: Actor identifier
  name: actorId
  type: string
- description: Total pending messages
  name: pendingCount
  type: integer
- description: ''
  name: messages
  type: array
- description: Age of oldest message in milliseconds
  name: oldestMessageAge
  type: integer
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-mailbox-inspection-schema.json
slug: actor-model-mailbox-inspection
source_filename: actor-model-mailbox-inspection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-mailboxinspection-schema.json\",\n  \"title\": \"MailboxInspection\",\n  \"description\": \"Inspection of pending messages in an actor's mailbox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actorId\": {\n      \"type\": \"string\",\n      \"description\": \"Actor identifier\",\n      \"example\": \"user-123\"\n    },\n    \"pendingCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total pending messages\",\n      \"example\": 5\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ActorMessage\"\n      }\n    },\n    \"oldestMessageAge\": {\n      \"type\": \"integer\",\n      \"description\": \"Age of oldest message in milliseconds\",\n      \"example\": 350\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-mailbox-inspection-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: MailboxInspection
---

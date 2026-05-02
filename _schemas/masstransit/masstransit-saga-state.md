---
description: Schema for MassTransit saga state machine instance data. Sagas coordinate long-running business processes across multiple services using a state machine pattern.
layout: schema
name: MassTransit Saga State
properties_list:
- description: Unique identifier that correlates all messages belonging to this saga instance
  name: correlationId
  type: string
- description: The current state of the saga state machine (e.g., Initial, Processing, Completed, Faulted)
  name: currentState
  type: string
- description: Optimistic concurrency version for the saga instance
  name: version
  type: integer
- description: Timestamp when the saga instance was created
  name: created
  type: string
- description: Timestamp of the last state transition
  name: updated
  type: string
- description: Row version for database concurrency (Entity Framework)
  name: rowVersion
  type: string
- description: Token ID for scheduled timeout events
  name: expirationTokenId
  type: string
- description: The message that caused the saga to fault, if applicable
  name: faultedMessage
  type: object
provider_name: MassTransit
provider_slug: masstransit
schema_file: json-schema/masstransit-saga-state.json
slug: masstransit-saga-state
source_filename: masstransit-saga-state.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/masstransit/masstransit-saga-state.json\",\n  \"title\": \"MassTransit Saga State\",\n  \"description\": \"Schema for MassTransit saga state machine instance data. Sagas coordinate long-running business processes across multiple services using a state machine pattern.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier that correlates all messages belonging to this saga instance\"\n    },\n    \"currentState\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the saga state machine (e.g., Initial, Processing, Completed, Faulted)\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Optimistic concurrency version for the saga instance\"\n    },\n    \"created\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the saga instance was created\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last state transition\"\n    },\n    \"rowVersion\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"description\": \"Row version for database concurrency (Entity Framework)\"\n    },\n    \"expirationTokenId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Token ID for scheduled timeout events\"\n    },\n    \"faultedMessage\": {\n      \"type\": \"object\",\n      \"description\": \"The message that caused the saga to fault, if applicable\",\n      \"properties\": {\n        \"messageType\": {\n          \"type\": \"string\"\n        },\n        \"message\": {\n          \"type\": \"object\"\n        },\n        \"exceptionType\": {\n          \"type\": \"string\"\n       \
  \ },\n        \"exceptionMessage\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"correlationId\", \"currentState\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/masstransit/refs/heads/main/json-schema/masstransit-saga-state.json
tags:
- .NET
- Event-Driven
- Message Bus
- Messaging
- Open Source
- Sagas
title: MassTransit Saga State
---

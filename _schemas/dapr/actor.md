---
description: Represents a Dapr virtual actor instance, including its type, identifier, and associated timer and reminder configurations.
layout: schema
name: Dapr Actor
properties_list:
- description: The type of the actor.
  name: actorType
  type: string
- description: The unique identifier of the actor instance.
  name: actorId
  type: string
- description: Timer configuration for the actor.
  name: timer
  type: object
- description: Persistent reminder configuration for the actor. Reminders survive actor deactivations and failovers.
  name: reminder
  type: object
provider_name: Dapr
provider_slug: dapr
schema_file: json-schema/actor.json
slug: actor
source_filename: actor.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/dapr/blob/main/json-schema/actor.json\",\n  \"title\": \"Dapr Actor\",\n  \"description\": \"Represents a Dapr virtual actor instance, including its type, identifier, and associated timer and reminder configurations.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"actorType\",\n    \"actorId\"\n  ],\n  \"properties\": {\n    \"actorType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the actor.\"\n    },\n    \"actorId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the actor instance.\"\n    },\n    \"timer\": {\n      \"type\": \"object\",\n      \"description\": \"Timer configuration for the actor.\",\n      \"properties\": {\n        \"dueTime\": {\n          \"type\": \"string\",\n          \"description\": \"Time after which the timer fires for the first time (ISO 8601 duration or time).\"\
  \n        },\n        \"period\": {\n          \"type\": \"string\",\n          \"description\": \"Time interval between timer fires (ISO 8601 duration).\"\n        },\n        \"callback\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the callback method to invoke.\"\n        },\n        \"data\": {\n          \"description\": \"Data to pass to the callback method.\"\n        }\n      }\n    },\n    \"reminder\": {\n      \"type\": \"object\",\n      \"description\": \"Persistent reminder configuration for the actor. Reminders survive actor deactivations and failovers.\",\n      \"properties\": {\n        \"dueTime\": {\n          \"type\": \"string\",\n          \"description\": \"Time after which the reminder fires for the first time.\"\n        },\n        \"period\": {\n          \"type\": \"string\",\n          \"description\": \"Time interval between reminder fires.\"\n        },\n        \"data\": {\n          \"description\": \"Data to pass to the\
  \ reminder callback.\"\n        },\n        \"ttl\": {\n          \"type\": \"string\",\n          \"description\": \"Time-to-live for the reminder.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/json-schema/actor.json
tags:
- Distributed Systems
- Microservices
- Platform
- Pub/Sub
- State Management
- Workflows
title: Dapr Actor
---

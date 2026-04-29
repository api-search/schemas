---
description: Request to spawn a new actor
layout: schema
name: SpawnActorRequest
properties_list:
- description: Behavior class or type name
  name: behavior
  type: string
- description: Optional custom actor ID (auto-generated if omitted)
  name: id
  type: string
- description: Parent supervisor ID
  name: supervisorId
  type: string
- description: Initial state to inject into the actor
  name: initialState
  type: object
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-spawn-actor-request-schema.json
slug: actor-model-spawn-actor-request
source_filename: actor-model-spawn-actor-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-spawnactorrequest-schema.json\",\n  \"title\": \"SpawnActorRequest\",\n  \"description\": \"Request to spawn a new actor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"behavior\": {\n      \"type\": \"string\",\n      \"description\": \"Behavior class or type name\",\n      \"example\": \"UserSessionBehavior\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Optional custom actor ID (auto-generated if omitted)\",\n      \"example\": \"session-abc\"\n    },\n    \"supervisorId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent supervisor ID\",\n      \"example\": \"session-supervisor\"\n    },\n    \"initialState\": {\n      \"type\": \"object\",\n      \"description\": \"Initial state to inject into the actor\",\n      \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-spawn-actor-request-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: SpawnActorRequest
---

---
description: A supervisor actor managing a set of child actors
layout: schema
name: Supervisor
properties_list:
- description: Supervisor actor ID
  name: id
  type: string
- description: Actor path
  name: path
  type: string
- description: Supervision strategy
  name: strategy
  type: string
- description: Maximum restart attempts within window
  name: maxRestarts
  type: integer
- description: Restart window in seconds
  name: restartWindow
  type: integer
- description: Current number of supervised children
  name: childCount
  type: integer
- description: Supervisor status
  name: status
  type: string
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-supervisor-schema.json
slug: actor-model-supervisor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-supervisor-schema.json\",\n  \"title\": \"Supervisor\",\n  \"description\": \"A supervisor actor managing a set of child actors\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Supervisor actor ID\",\n      \"example\": \"session-supervisor\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Actor path\",\n      \"example\": \"/system/supervisor/session-supervisor\"\n    },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"one-for-one\",\n        \"one-for-all\",\n        \"rest-for-one\",\n        \"all-for-one\"\n      ],\n      \"description\": \"Supervision strategy\",\n      \"example\": \"one-for-one\"\n    },\n    \"maxRestarts\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum restart attempts\
  \ within window\",\n      \"example\": 10\n    },\n    \"restartWindow\": {\n      \"type\": \"integer\",\n      \"description\": \"Restart window in seconds\",\n      \"example\": 60\n    },\n    \"childCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Current number of supervised children\",\n      \"example\": 42\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Supervisor status\",\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-supervisor-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: Supervisor
---

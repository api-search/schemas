---
description: Paginated list of supervisors
layout: schema
name: SupervisorList
properties_list:
- description: ''
  name: supervisors
  type: array
- description: Total supervisor count
  name: total
  type: integer
- description: Cursor for next page
  name: cursor
  type: string
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-supervisor-list-schema.json
slug: actor-model-supervisor-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-supervisorlist-schema.json\",\n  \"title\": \"SupervisorList\",\n  \"description\": \"Paginated list of supervisors\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"supervisors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Supervisor\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total supervisor count\",\n      \"example\": 12\n    },\n    \"cursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for next page\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-supervisor-list-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: SupervisorList
---

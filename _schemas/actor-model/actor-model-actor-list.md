---
description: Paginated list of actors
layout: schema
name: ActorList
properties_list:
- description: ''
  name: actors
  type: array
- description: Total actor count
  name: total
  type: integer
- description: Cursor for next page
  name: cursor
  type: string
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-actor-list-schema.json
slug: actor-model-actor-list
source_filename: actor-model-actor-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-actorlist-schema.json\",\n  \"title\": \"ActorList\",\n  \"description\": \"Paginated list of actors\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Actor\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total actor count\",\n      \"example\": 500\n    },\n    \"cursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for next page\",\n      \"example\": \"eyJwYWdlIjoxfQ==\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-actor-list-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: ActorList
---

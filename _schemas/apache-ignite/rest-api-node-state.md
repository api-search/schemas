---
description: Node state.
layout: schema
name: NodeState
properties_list:
- description: Unique node name.
  name: name
  type: string
- description: ''
  name: state
  type: object
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-node-state-schema.json
slug: rest-api-node-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-state-schema.json\",\n  \"title\": \"NodeState\",\n  \"description\": \"Node state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique node name.\"\n    },\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"Node state.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-node-state-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: NodeState
---

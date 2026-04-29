---
description: Rest representation of transaction.
layout: schema
name: Transaction
properties_list:
- description: Transaction ID.
  name: id
  type: string
- description: Coordinator node.
  name: node
  type: string
- description: State.
  name: state
  type: string
- description: Type.
  name: type
  type: string
- description: Priority.
  name: priority
  type: string
- description: Start time.
  name: startTime
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-transaction-schema.json
slug: rest-api-transaction
source_filename: rest-api-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"description\": \"Rest representation of transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction ID.\",\n      \"format\": \"uuid\"\n    },\n    \"node\": {\n      \"type\": \"string\",\n      \"description\": \"Coordinator node.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type.\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Priority.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"Start time.\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"\
  required\": [\n    \"id\",\n    \"node\",\n    \"priority\",\n    \"startTime\",\n    \"state\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-transaction-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: Transaction
---

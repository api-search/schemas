---
description: A sync session used to upload batches of entity data to Zluri. Only one sync can be active per instance at a time.
layout: schema
name: Zluri Sync Session
properties_list:
- description: Unique identifier of the sync session.
  name: id
  type: string
- description: The instance this sync belongs to.
  name: instance_id
  type: string
- description: Current status of the sync.
  name: status
  type: string
- description: When the sync was created.
  name: created_at
  type: string
- description: When the sync was finished. Null if still running.
  name: finished_at
  type:
  - string
  - 'null'
provider_name: Zluri
provider_slug: zluri
schema_file: json-schema/sync.json
slug: sync
source_filename: sync.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/sync.json\",\n  \"title\": \"Zluri Sync Session\",\n  \"description\": \"A sync session used to upload batches of entity data to Zluri. Only one sync can be active per instance at a time.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the sync session.\"\n    },\n    \"instance_id\": {\n      \"type\": \"string\",\n      \"description\": \"The instance this sync belongs to.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the sync.\",\n      \"enum\": [\"running\", \"finished\", \"failed\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the sync was created.\"\n    },\n    \"finished_at\": {\n\
  \      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the sync was finished. Null if still running.\"\n    }\n  },\n  \"required\": [\"id\", \"instance_id\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/sync.json
tags:
- Access Management
- SaaS Management
title: Zluri Sync Session
---

---
description: A public workflow within the Cobalt embedded integration platform.
layout: schema
name: Workflow
properties_list:
- description: Workflow ID.
  name: _id
  type: string
- description: Workflow name.
  name: name
  type: string
- description: Workflow description.
  name: description
  type: string
- description: Workflow nodes.
  name: nodes
  type: array
- description: Creation timestamp.
  name: created_at
  type: string
- description: Last update timestamp.
  name: updated_at
  type: string
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/workflow.json
slug: workflow
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/workflow.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Workflow\",\n  \"description\": \"A public workflow within the Cobalt embedded integration platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Workflow ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Workflow name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Workflow description.\"\n    },\n    \"nodes\": {\n      \"type\": \"array\",\n      \"description\": \"Workflow nodes.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"config\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n   \
  \ },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/workflow.json
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Workflow
---

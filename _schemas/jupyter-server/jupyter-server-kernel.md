---
description: Schema for a kernel resource as returned by the Jupyter Server REST API.
layout: schema
name: Jupyter Server Kernel
properties_list:
- description: Unique kernel identifier (UUID).
  name: id
  type: string
- description: Kernel spec name (for example python3).
  name: name
  type: string
- description: ISO 8601 timestamp of the last kernel activity.
  name: last_activity
  type: string
- description: Current execution state of the kernel.
  name: execution_state
  type: string
- description: Number of clients connected to this kernel.
  name: connections
  type: integer
provider_name: Jupyter Server
provider_slug: jupyter-server
schema_file: json-schema/jupyter-server-kernel.json
slug: jupyter-server-kernel
source_filename: jupyter-server-kernel.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyter-server/main/json-schema/jupyter-server-kernel.json\",\n  \"title\": \"Jupyter Server Kernel\",\n  \"description\": \"Schema for a kernel resource as returned by the Jupyter Server REST API.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique kernel identifier (UUID).\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Kernel spec name (for example python3).\"\n    },\n    \"last_activity\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last kernel activity.\"\n    },\n    \"execution_state\": {\n      \"type\": \"string\",\n      \"enum\": [\"starting\", \"idle\", \"busy\", \"terminating\", \"restarting\", \"autorestarting\", \"\
  dead\"],\n      \"description\": \"Current execution state of the kernel.\"\n    },\n    \"connections\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of clients connected to this kernel.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/json-schema/jupyter-server-kernel.json
tags:
- Compute
- Interactive Computing
- Kernels
- Notebooks
- Portable
- Workbooks
title: Jupyter Server Kernel
---

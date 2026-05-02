---
description: Schema for a Jupyter Server session, which binds a notebook or file to a kernel.
layout: schema
name: Jupyter Server Session
properties_list:
- description: Unique session identifier (UUID).
  name: id
  type: string
- description: Path to the document associated with the session.
  name: path
  type: string
- description: Name of the session.
  name: name
  type: string
- description: Type of the session (for example notebook, console).
  name: type
  type: string
- description: ''
  name: kernel
  type: object
provider_name: Jupyter Server
provider_slug: jupyter-server
schema_file: json-schema/jupyter-server-session.json
slug: jupyter-server-session
source_filename: jupyter-server-session.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyter-server/main/json-schema/jupyter-server-session.json\",\n  \"title\": \"Jupyter Server Session\",\n  \"description\": \"Schema for a Jupyter Server session, which binds a notebook or file to a kernel.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"kernel\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique session identifier (UUID).\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the document associated with the session.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the session.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the session (for example notebook, console).\"\n    },\n    \"kernel\": {\n      \"$ref\": \"jupyter-server-kernel.json\"\n    }\n \
  \ }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/json-schema/jupyter-server-session.json
tags:
- Compute
- Interactive Computing
- Kernels
- Notebooks
- Portable
- Workbooks
title: Jupyter Server Session
---

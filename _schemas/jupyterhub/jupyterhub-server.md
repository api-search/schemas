---
description: Schema for a JupyterHub single-user server resource.
layout: schema
name: JupyterHub Server
properties_list:
- description: Server name (empty string for the default server).
  name: name
  type: string
- description: Whether the server is ready to handle requests.
  name: ready
  type: boolean
- description: Whether the server is stopped.
  name: stopped
  type: boolean
- description: Pending action on this server.
  name: pending
  type:
  - string
  - 'null'
- description: URL where the server is reachable.
  name: url
  type: string
- description: URL for the server's spawn progress events.
  name: progress_url
  type: string
- description: When the server was started.
  name: started
  type:
  - string
  - 'null'
- description: Last activity timestamp on the server.
  name: last_activity
  type:
  - string
  - 'null'
- description: Spawner-specific state.
  name: state
  type: object
- description: Spawner user options used to start the server.
  name: user_options
  type: object
provider_name: JupyterHub
provider_slug: jupyterhub
schema_file: json-schema/jupyterhub-server.json
slug: jupyterhub-server
source_filename: jupyterhub-server.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyterhub/main/json-schema/jupyterhub-server.json\",\n  \"title\": \"JupyterHub Server\",\n  \"description\": \"Schema for a JupyterHub single-user server resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Server name (empty string for the default server).\"\n    },\n    \"ready\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the server is ready to handle requests.\"\n    },\n    \"stopped\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the server is stopped.\"\n    },\n    \"pending\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"spawn\", \"stop\", null],\n      \"description\": \"Pending action on this server.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL where the server\
  \ is reachable.\"\n    },\n    \"progress_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL for the server's spawn progress events.\"\n    },\n    \"started\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the server was started.\"\n    },\n    \"last_activity\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Last activity timestamp on the server.\"\n    },\n    \"state\": {\n      \"type\": \"object\",\n      \"description\": \"Spawner-specific state.\"\n    },\n    \"user_options\": {\n      \"type\": \"object\",\n      \"description\": \"Spawner user options used to start the server.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/json-schema/jupyterhub-server.json
tags:
- Authentication
- Data Science
- Education
- Hub
- Multi-User
- Notebooks
- OAuth2
- Python
title: JupyterHub Server
---

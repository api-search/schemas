---
description: Schema for a JupyterHub user resource.
layout: schema
name: JupyterHub User
properties_list:
- description: The user name.
  name: name
  type: string
- description: Whether the user has admin privileges.
  name: admin
  type: boolean
- description: Roles assigned to the user.
  name: roles
  type: array
- description: Groups the user belongs to.
  name: groups
  type: array
- description: URL of the user's default server, or null if not running.
  name: server
  type:
  - string
  - 'null'
- description: Pending action on the user's server.
  name: pending
  type:
  - string
  - 'null'
- description: When the user account was created.
  name: created
  type: string
- description: Last activity timestamp for the user.
  name: last_activity
  type:
  - string
  - 'null'
- description: Mapping of named server names to server objects.
  name: servers
  type: object
provider_name: JupyterHub
provider_slug: jupyterhub
schema_file: json-schema/jupyterhub-user.json
slug: jupyterhub-user
source_filename: jupyterhub-user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyterhub/main/json-schema/jupyterhub-user.json\",\n  \"title\": \"JupyterHub User\",\n  \"description\": \"Schema for a JupyterHub user resource.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The user name.\"\n    },\n    \"admin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has admin privileges.\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\"type\": \"string\"},\n      \"description\": \"Roles assigned to the user.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {\"type\": \"string\"},\n      \"description\": \"Groups the user belongs to.\"\n    },\n    \"server\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"URL of the user's default\
  \ server, or null if not running.\"\n    },\n    \"pending\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"spawn\", \"stop\", null],\n      \"description\": \"Pending action on the user's server.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the user account was created.\"\n    },\n    \"last_activity\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Last activity timestamp for the user.\"\n    },\n    \"servers\": {\n      \"type\": \"object\",\n      \"description\": \"Mapping of named server names to server objects.\",\n      \"additionalProperties\": {\"$ref\": \"jupyterhub-server.json\"}\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/json-schema/jupyterhub-user.json
tags:
- Authentication
- Data Science
- Education
- Hub
- Multi-User
- Notebooks
- OAuth2
- Python
title: JupyterHub User
---

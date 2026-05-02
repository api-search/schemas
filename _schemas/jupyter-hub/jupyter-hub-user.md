---
description: Schema for a JupyterHub user as exposed by the Hub REST API.
layout: schema
name: JupyterHub User
properties_list:
- description: Username.
  name: name
  type: string
- description: Whether the user is an administrator.
  name: admin
  type: boolean
- description: Group memberships.
  name: groups
  type: array
- description: URL of the user's default server, if running.
  name: server
  type:
  - string
  - 'null'
- description: Pending state of the default server, if any.
  name: pending
  type:
  - string
  - 'null'
- description: ''
  name: created
  type: string
- description: ''
  name: last_activity
  type:
  - string
  - 'null'
- description: ''
  name: servers
  type: object
- description: ''
  name: kind
  type: string
provider_name: JupyterHub
provider_slug: jupyter-hub
schema_file: json-schema/jupyter-hub-user.json
slug: jupyter-hub-user
source_filename: jupyter-hub-user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyter-hub/main/json-schema/jupyter-hub-user.json\",\n  \"title\": \"JupyterHub User\",\n  \"description\": \"Schema for a JupyterHub user as exposed by the Hub REST API.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": { \"type\": \"string\", \"description\": \"Username.\" },\n    \"admin\": { \"type\": \"boolean\", \"description\": \"Whether the user is an administrator.\" },\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Group memberships.\"\n    },\n    \"server\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"URL of the user's default server, if running.\"\n    },\n    \"pending\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"spawn\", \"stop\", null],\n      \"description\": \"Pending state\
  \ of the default server, if any.\"\n    },\n    \"created\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"last_activity\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" },\n    \"servers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"ready\": { \"type\": \"boolean\" },\n          \"started\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" },\n          \"url\": { \"type\": \"string\" },\n          \"user_options\": { \"type\": \"object\" },\n          \"progress_url\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"enum\": [\"user\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyter-hub/refs/heads/main/json-schema/jupyter-hub-user.json
tags:
- Data Science
- Education
- Jupyter
- Multi-User
- Notebooks
title: JupyterHub User
---

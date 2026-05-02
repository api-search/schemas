---
description: Schema for a JupyterHub group resource.
layout: schema
name: JupyterHub Group
properties_list:
- description: The group name.
  name: name
  type: string
- description: User names that belong to the group.
  name: users
  type: array
- description: Roles assigned to the group.
  name: roles
  type: array
- description: Arbitrary group properties.
  name: properties
  type: object
provider_name: JupyterHub
provider_slug: jupyterhub
schema_file: json-schema/jupyterhub-group.json
slug: jupyterhub-group
source_filename: jupyterhub-group.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyterhub/main/json-schema/jupyterhub-group.json\",\n  \"title\": \"JupyterHub Group\",\n  \"description\": \"Schema for a JupyterHub group resource.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The group name.\"\n    },\n    \"users\": {\n      \"type\": \"array\",\n      \"items\": {\"type\": \"string\"},\n      \"description\": \"User names that belong to the group.\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\"type\": \"string\"},\n      \"description\": \"Roles assigned to the group.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary group properties.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/json-schema/jupyterhub-group.json
tags:
- Authentication
- Data Science
- Education
- Hub
- Multi-User
- Notebooks
- OAuth2
- Python
title: JupyterHub Group
---

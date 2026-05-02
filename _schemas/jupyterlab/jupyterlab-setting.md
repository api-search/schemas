---
description: Schema for a JupyterLab plugin setting document returned from the settings REST API.
layout: schema
name: JupyterLab Plugin Setting
properties_list:
- description: Plugin identifier (for example @jupyterlab/apputils-extension:themes).
  name: id
  type: string
- description: Raw JSON5 settings document submitted by the user.
  name: raw
  type: string
- description: JSON Schema describing valid settings for the plugin.
  name: schema
  type: object
- description: Effective settings, merged from the user values and the schema defaults.
  name: settings
  type: object
- description: Plugin version associated with the schema.
  name: version
  type: string
- description: Timestamp the setting was last modified.
  name: last_modified
  type: string
- description: Timestamp the setting was first created.
  name: created
  type: string
provider_name: JupyterLab
provider_slug: jupyterlab
schema_file: json-schema/jupyterlab-setting.json
slug: jupyterlab-setting
source_filename: jupyterlab-setting.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyterlab/main/json-schema/jupyterlab-setting.json\",\n  \"title\": \"JupyterLab Plugin Setting\",\n  \"description\": \"Schema for a JupyterLab plugin setting document returned from the settings REST API.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"raw\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Plugin identifier (for example @jupyterlab/apputils-extension:themes).\"\n    },\n    \"raw\": {\n      \"type\": \"string\",\n      \"description\": \"Raw JSON5 settings document submitted by the user.\"\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"JSON Schema describing valid settings for the plugin.\"\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"Effective settings, merged from the user values and the schema defaults.\"\
  \n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Plugin version associated with the schema.\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp the setting was last modified.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp the setting was first created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyterlab/refs/heads/main/json-schema/jupyterlab-setting.json
tags:
- Data Science
- Extensions
- IDE
- Interactive Computing
- Notebooks
- Python
title: JupyterLab Plugin Setting
---

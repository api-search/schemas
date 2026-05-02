---
description: Schema for a JupyterLab workspace, persisted via the workspaces REST API.
layout: schema
name: JupyterLab Workspace
properties_list:
- description: Workspace layout data, keyed by JupyterLab plugin identifiers.
  name: data
  type: object
- description: ''
  name: metadata
  type: object
provider_name: JupyterLab
provider_slug: jupyterlab
schema_file: json-schema/jupyterlab-workspace.json
slug: jupyterlab-workspace
source_filename: jupyterlab-workspace.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyterlab/main/json-schema/jupyterlab-workspace.json\",\n  \"title\": \"JupyterLab Workspace\",\n  \"description\": \"Schema for a JupyterLab workspace, persisted via the workspaces REST API.\",\n  \"type\": \"object\",\n  \"required\": [\"data\", \"metadata\"],\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Workspace layout data, keyed by JupyterLab plugin identifiers.\",\n      \"additionalProperties\": true\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique workspace identifier.\"\n        },\n        \"last_modified\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the last modification.\"\
  \n        },\n        \"created\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp the workspace was created.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyterlab/refs/heads/main/json-schema/jupyterlab-workspace.json
tags:
- Data Science
- Extensions
- IDE
- Interactive Computing
- Notebooks
- Python
title: JupyterLab Workspace
---

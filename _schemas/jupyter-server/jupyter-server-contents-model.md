---
description: Schema for the contents model returned by the Jupyter Server REST API for files, directories, and notebooks.
layout: schema
name: Jupyter Server Contents Model
properties_list:
- description: Basename of the entity.
  name: name
  type: string
- description: Full path of the entity, relative to the server root.
  name: path
  type: string
- description: Kind of contents.
  name: type
  type: string
- description: Whether the entity is writable.
  name: writable
  type: boolean
- description: Creation timestamp.
  name: created
  type: string
- description: Last modified timestamp.
  name: last_modified
  type: string
- description: MIME type of the file (null for directories and notebooks).
  name: mimetype
  type:
  - string
  - 'null'
- description: File contents, directory listing, or notebook JSON. Null when content is not requested.
  name: content
  type: object
- description: Encoding of the content.
  name: format
  type:
  - string
  - 'null'
- description: Size of the entity in bytes.
  name: size
  type:
  - integer
  - 'null'
- description: Hash of the file contents.
  name: hash
  type:
  - string
  - 'null'
provider_name: Jupyter Server
provider_slug: jupyter-server
schema_file: json-schema/jupyter-server-contents-model.json
slug: jupyter-server-contents-model
source_filename: jupyter-server-contents-model.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/jupyter-server/main/json-schema/jupyter-server-contents-model.json\",\n  \"title\": \"Jupyter Server Contents Model\",\n  \"description\": \"Schema for the contents model returned by the Jupyter Server REST API for files, directories, and notebooks.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"path\", \"type\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Basename of the entity.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Full path of the entity, relative to the server root.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"file\", \"directory\", \"notebook\"],\n      \"description\": \"Kind of contents.\"\n    },\n    \"writable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the entity is writable.\"\
  \n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp.\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modified timestamp.\"\n    },\n    \"mimetype\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"MIME type of the file (null for directories and notebooks).\"\n    },\n    \"content\": {\n      \"description\": \"File contents, directory listing, or notebook JSON. Null when content is not requested.\"\n    },\n    \"format\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"text\", \"base64\", \"json\", null],\n      \"description\": \"Encoding of the content.\"\n    },\n    \"size\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Size of the entity in bytes.\"\n    },\n    \"hash\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Hash of the file\
  \ contents.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyter-server/refs/heads/main/json-schema/jupyter-server-contents-model.json
tags:
- Compute
- Interactive Computing
- Kernels
- Notebooks
- Portable
- Workbooks
title: Jupyter Server Contents Model
---

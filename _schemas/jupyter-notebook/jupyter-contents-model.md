---
description: Schema for the Jupyter Contents API model representing files, directories, and notebooks in the Jupyter file system. This is the primary data structure returned by the Contents REST API.
layout: schema
name: Jupyter Contents Model
properties_list:
- description: Name of the file or directory (e.g., 'Untitled.ipynb').
  name: name
  type: string
- description: Full path relative to the root directory (e.g., 'path/to/Untitled.ipynb').
  name: path
  type: string
- description: Type of content.
  name: type
  type: string
- description: Whether the requester has write permission.
  name: writable
  type: boolean
- description: Creation timestamp in ISO 8601 format.
  name: created
  type: string
- description: Last modification timestamp in ISO 8601 format.
  name: last_modified
  type: string
- description: Size in bytes. Null for directories and notebooks.
  name: size
  type:
  - integer
  - 'null'
- description: MIME type of the content. Null for directories and notebooks.
  name: mimetype
  type:
  - string
  - 'null'
- description: The content itself. For directories, an array of contents models (without content). For notebooks, the notebook JSON object. For files, a string (text) or base64-encoded string.
  name: content
  type: object
- description: Format of the content field.
  name: format
  type:
  - string
  - 'null'
- description: Hash of the file content for change detection.
  name: hash
  type:
  - string
  - 'null'
- description: Algorithm used to compute the hash (e.g., 'sha256').
  name: hash_algorithm
  type:
  - string
  - 'null'
provider_name: Jupyter Notebook
provider_slug: jupyter-notebook
schema_file: json-schema/jupyter-contents-model.json
slug: jupyter-contents-model
source_filename: jupyter-contents-model.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"jupyter-contents-model.json\",\n  \"title\": \"Jupyter Contents Model\",\n  \"description\": \"Schema for the Jupyter Contents API model representing files, directories, and notebooks in the Jupyter file system. This is the primary data structure returned by the Contents REST API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the file or directory (e.g., 'Untitled.ipynb').\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Full path relative to the root directory (e.g., 'path/to/Untitled.ipynb').\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of content.\",\n      \"enum\": [\"notebook\", \"file\", \"directory\"]\n    },\n    \"writable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the requester has write permission.\"\n\
  \    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp in ISO 8601 format.\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp in ISO 8601 format.\"\n    },\n    \"size\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Size in bytes. Null for directories and notebooks.\",\n      \"minimum\": 0\n    },\n    \"mimetype\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"MIME type of the content. Null for directories and notebooks.\"\n    },\n    \"content\": {\n      \"description\": \"The content itself. For directories, an array of contents models (without content). For notebooks, the notebook JSON object. For files, a string (text) or base64-encoded string.\"\n    },\n    \"format\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Format of the\
  \ content field.\",\n      \"enum\": [\"json\", \"text\", \"base64\", null]\n    },\n    \"hash\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Hash of the file content for change detection.\"\n    },\n    \"hash_algorithm\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Algorithm used to compute the hash (e.g., 'sha256').\"\n    }\n  },\n  \"required\": [\"name\", \"path\", \"type\", \"writable\", \"created\", \"last_modified\"],\n  \"if\": {\n    \"properties\": {\n      \"type\": {\"const\": \"directory\"}\n    }\n  },\n  \"then\": {\n    \"properties\": {\n      \"content\": {\n        \"type\": [\"array\", \"null\"],\n        \"items\": {\n          \"$ref\": \"#\"\n        }\n      },\n      \"format\": {\n        \"const\": \"json\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jupyter-notebook/refs/heads/main/json-schema/jupyter-contents-model.json
tags:
- Data Science
- Interactive Computing
- Jupyter
- Machine Learning
- Notebooks
- Python
title: Jupyter Contents Model
---

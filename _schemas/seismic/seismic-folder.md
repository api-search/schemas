---
description: A content folder in the Seismic platform used to organize content items in a hierarchical structure.
layout: schema
name: Seismic Folder
properties_list:
- description: Unique identifier of the folder.
  name: id
  type: string
- description: Name of the folder.
  name: name
  type: string
- description: Description of the folder.
  name: description
  type: string
- description: ID of the parent folder. Null for root-level folders.
  name: parentId
  type:
  - string
  - 'null'
- description: Full path of the folder in the folder hierarchy.
  name: path
  type: string
- description: Number of content items in the folder.
  name: contentCount
  type: integer
- description: Number of child folders.
  name: childFolderCount
  type: integer
- description: ID of the user who created the folder.
  name: createdBy
  type: string
- description: Timestamp when the folder was created.
  name: createdAt
  type: string
- description: ID of the user who last modified the folder.
  name: modifiedBy
  type: string
- description: Timestamp when the folder was last modified.
  name: modifiedAt
  type: string
provider_name: Seismic
provider_slug: seismic
schema_file: json-schema/seismic-folder-schema.json
slug: seismic-folder
source_filename: seismic-folder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.seismic.com/schemas/folder\",\n  \"title\": \"Seismic Folder\",\n  \"description\": \"A content folder in the Seismic platform used to organize content items in a hierarchical structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the folder.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the folder.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the folder.\"\n    },\n    \"parentId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the parent folder. Null for root-level folders.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Full path of the folder in the folder hierarchy.\"\n    },\n    \"contentCount\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Number of content items in the folder.\",\n      \"minimum\": 0\n    },\n    \"childFolderCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of child folders.\",\n      \"minimum\": 0\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created the folder.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the folder was created.\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified the folder.\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the folder was last modified.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/json-schema/seismic-folder-schema.json
tags: []
title: Seismic Folder
---

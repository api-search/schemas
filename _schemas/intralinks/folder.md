---
description: A folder within an Intralinks workspace used to organize documents in a hierarchical structure with index-based ordering.
layout: schema
name: Intralinks Folder
properties_list:
- description: Unique identifier of the folder.
  name: id
  type: string
- description: Folder name.
  name: name
  type: string
- description: ID of the parent folder.
  name: parentId
  type: string
- description: Index number for folder ordering.
  name: indexNumber
  type: string
- description: Whether the folder contains subfolders.
  name: hasChildFolders
  type: boolean
- description: Version number of the folder.
  name: version
  type: integer
- description: Folder creation timestamp.
  name: createdOn
  type: string
- description: Last modification timestamp.
  name: updatedOn
  type: string
provider_name: Intralinks
provider_slug: intralinks
schema_file: json-schema/folder.json
slug: folder
source_filename: folder.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"folder.json\",\n  \"title\": \"Intralinks Folder\",\n  \"description\": \"A folder within an Intralinks workspace used to organize documents in a hierarchical structure with index-based ordering.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the folder.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Folder name.\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent folder.\"\n    },\n    \"indexNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Index number for folder ordering.\"\n    },\n    \"hasChildFolders\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the folder contains subfolders.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number\
  \ of the folder.\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Folder creation timestamp.\"\n    },\n    \"updatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/json-schema/folder.json
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
title: Intralinks Folder
---

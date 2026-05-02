---
description: A document stored within an Intralinks workspace, representing a file with associated metadata, versioning, and access control.
layout: schema
name: Intralinks Document
properties_list:
- description: Unique identifier of the document.
  name: id
  type: string
- description: Document name.
  name: name
  type: string
- description: ID of the containing folder.
  name: folderId
  type: string
- description: File size in bytes.
  name: fileSize
  type: integer
- description: File extension (e.g., pdf, docx).
  name: extension
  type: string
- description: Version number of the document.
  name: version
  type: integer
- description: Document note or description.
  name: note
  type: string
- description: User who created the document.
  name: createdBy
  type: string
- description: Document creation timestamp.
  name: createdOn
  type: string
- description: Last modification timestamp.
  name: updatedOn
  type: string
- description: Timestamp of last access.
  name: lastAccessedOn
  type: string
provider_name: Intralinks
provider_slug: intralinks
schema_file: json-schema/document.json
slug: document
source_filename: document.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"document.json\",\n  \"title\": \"Intralinks Document\",\n  \"description\": \"A document stored within an Intralinks workspace, representing a file with associated metadata, versioning, and access control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the document.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Document name.\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the containing folder.\"\n    },\n    \"fileSize\": {\n      \"type\": \"integer\",\n      \"description\": \"File size in bytes.\"\n    },\n    \"extension\": {\n      \"type\": \"string\",\n      \"description\": \"File extension (e.g., pdf, docx).\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the\
  \ document.\"\n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"description\": \"Document note or description.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the document.\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Document creation timestamp.\"\n    },\n    \"updatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp.\"\n    },\n    \"lastAccessedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last access.\"\n    }\n  },\n  \"required\": [\"name\", \"folderId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/json-schema/document.json
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
title: Intralinks Document
---

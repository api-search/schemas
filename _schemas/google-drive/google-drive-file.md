---
description: JSON Schema for a Google Drive file resource as returned by the Google Drive REST API v3.
layout: schema
name: Google Drive File
properties_list:
- description: The ID of the file.
  name: id
  type: string
- description: The name of the file.
  name: name
  type: string
- description: The MIME type of the file.
  name: mimeType
  type: string
- description: The IDs of the parent folders containing the file.
  name: parents
  type: array
- description: The time at which the file was created.
  name: createdTime
  type: string
- description: The last time the file was modified.
  name: modifiedTime
  type: string
- description: The size of the file's content in bytes.
  name: size
  type: string
- description: Whether the file has been trashed.
  name: trashed
  type: boolean
- description: Whether the user has starred the file.
  name: starred
  type: boolean
- description: Whether the file has been shared.
  name: shared
  type: boolean
- description: A link for opening the file in the relevant Google editor or viewer.
  name: webViewLink
  type: string
- description: A link for downloading the content of the file.
  name: webContentLink
  type: string
- description: A static, unauthenticated link to the file's icon.
  name: iconLink
  type: string
- description: The owners of the file.
  name: owners
  type: array
provider_name: Google Drive
provider_slug: google-drive
schema_file: json-schema/google-drive-file-schema.json
slug: google-drive-file
source_filename: google-drive-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-drive/refs/heads/main/json-schema/google-drive-file-schema.json\",\n  \"title\": \"Google Drive File\",\n  \"description\": \"JSON Schema for a Google Drive file resource as returned by the Google Drive REST API v3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the file.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file.\"\n    },\n    \"mimeType\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the file.\"\n    },\n    \"parents\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of the parent folders containing the file.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\",\n      \"description\": \"The time at which the file was created.\"\n    },\n    \"modifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last time the file was modified.\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"The size of the file's content in bytes.\"\n    },\n    \"trashed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the file has been trashed.\"\n    },\n    \"starred\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has starred the file.\"\n    },\n    \"shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the file has been shared.\"\n    },\n    \"webViewLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A link for opening the file in the relevant Google editor or viewer.\"\n    },\n    \"webContentLink\": {\n      \"type\": \"string\",\n      \"format\": \"\
  uri\",\n      \"description\": \"A link for downloading the content of the file.\"\n    },\n    \"iconLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A static, unauthenticated link to the file's icon.\"\n    },\n    \"owners\": {\n      \"type\": \"array\",\n      \"description\": \"The owners of the file.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayName\": {\"type\": \"string\"},\n          \"emailAddress\": {\"type\": \"string\"},\n          \"permissionId\": {\"type\": \"string\"}\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\", \"mimeType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-drive/refs/heads/main/json-schema/google-drive-file-schema.json
tags:
- Cloud Storage
- Collaboration
- Document Management
- Drive
- Files
- Google
- Storage
title: Google Drive File
---

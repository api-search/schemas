---
description: Represents a file, folder, or other item stored in a drive.
layout: schema
name: DriveItem
properties_list:
- description: The unique identifier of the item within the drive.
  name: id
  type: string
- description: The name of the item (filename and extension).
  name: name
  type: string
- description: A user-visible description of the item.
  name: description
  type: string
- description: Size of the item in bytes.
  name: size
  type: integer
- description: URL that displays the resource in the browser.
  name: webUrl
  type: string
- description: WebDAV compatible URL for the item.
  name: webDavUrl
  type: string
- description: Date and time of item creation.
  name: createdDateTime
  type: string
- description: Date and time the item was last modified.
  name: lastModifiedDateTime
  type: string
- description: ETag for the entire item.
  name: eTag
  type: string
- description: ETag for the content of the item.
  name: cTag
  type: string
- description: ''
  name: createdBy
  type: object
- description: ''
  name: lastModifiedBy
  type: object
- description: ''
  name: parentReference
  type: object
- description: ''
  name: file
  type: object
- description: ''
  name: folder
  type: object
provider_name: Microsoft Word
provider_slug: microsoft-word
schema_file: json-schema/graph-api-drive-item-schema.json
slug: graph-api-drive-item
source_filename: graph-api-drive-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/graph-api-drive-item-schema.json\",\n  \"title\": \"DriveItem\",\n  \"description\": \"Represents a file, folder, or other item stored in a drive.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the item within the drive.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the item (filename and extension).\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A user-visible description of the item.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Size of the item in bytes.\"\n    },\n    \"webUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\"\
  : \"URL that displays the resource in the browser.\"\n    },\n    \"webDavUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"WebDAV compatible URL for the item.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of item creation.\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the item was last modified.\"\n    },\n    \"eTag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for the entire item.\"\n    },\n    \"cTag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for the content of the item.\"\n    },\n    \"createdBy\": {\n      \"$ref\": \"#/$defs/IdentitySet\"\n    },\n    \"lastModifiedBy\": {\n      \"$ref\": \"#/$defs/IdentitySet\"\n    },\n    \"parentReference\": {\n      \"$ref\": \"#/$defs/ItemReference\"\n    },\n   \
  \ \"file\": {\n      \"$ref\": \"#/$defs/FileFacet\"\n    },\n    \"folder\": {\n      \"$ref\": \"#/$defs/FolderFacet\"\n    }\n  },\n  \"$defs\": {\n    \"IdentitySet\": {\n      \"type\": \"object\",\n      \"description\": \"Keyed collection of identity resources.\",\n      \"properties\": {\n        \"user\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": { \"type\": \"string\" },\n            \"displayName\": { \"type\": \"string\" }\n          }\n        }\n      }\n    },\n    \"ItemReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a drive item's parent.\",\n      \"properties\": {\n        \"driveId\": { \"type\": \"string\" },\n        \"id\": { \"type\": \"string\" },\n        \"path\": { \"type\": \"string\" }\n      }\n    },\n    \"FileFacet\": {\n      \"type\": \"object\",\n      \"description\": \"File metadata facet.\",\n      \"properties\": {\n        \"mimeType\": { \"type\": \"string\" },\n   \
  \     \"hashes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"sha1Hash\": { \"type\": \"string\" },\n            \"quickXorHash\": { \"type\": \"string\" }\n          }\n        }\n      }\n    },\n    \"FolderFacet\": {\n      \"type\": \"object\",\n      \"description\": \"Folder metadata facet.\",\n      \"properties\": {\n        \"childCount\": { \"type\": \"integer\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/graph-api-drive-item-schema.json
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
title: DriveItem
---

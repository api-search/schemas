---
description: ''
layout: schema
name: AlbumPayload
properties_list:
- description: Display name of the album
  name: name
  type: string
- description: When the user created the album
  name: userCreated
  type: string
- description: When the user last modified the album
  name: userUpdated
  type: string
- description: Cover asset for the album
  name: cover
  type: object
- description: Parent album reference for nested albums
  name: parent
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-albums-album-payload-schema.json
slug: lightroom-albums-album-payload
source_filename: lightroom-albums-album-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlbumPayload\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the album\"\n    },\n    \"userCreated\": {\n      \"type\": \"string\",\n      \"description\": \"When the user created the album\"\n    },\n    \"userUpdated\": {\n      \"type\": \"string\",\n      \"description\": \"When the user last modified the album\"\n    },\n    \"cover\": {\n      \"type\": \"object\",\n      \"description\": \"Cover asset for the album\"\n    },\n    \"parent\": {\n      \"type\": \"object\",\n      \"description\": \"Parent album reference for nested albums\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-albums-album-payload-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: AlbumPayload
---

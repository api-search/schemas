---
description: ''
layout: schema
name: Album
properties_list:
- description: Unique identifier of the album
  name: id
  type: string
- description: Resource type
  name: type
  type: string
- description: Album subtype
  name: subtype
  type: string
- description: Album creation timestamp
  name: created
  type: string
- description: Album last updated timestamp
  name: updated
  type: string
- description: Album payload data
  name: payload
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-services-album-schema.json
slug: lightroom-services-album
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Album\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the album\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type\"\n    },\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"Album subtype\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"Album creation timestamp\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"description\": \"Album last updated timestamp\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Album payload data\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-services-album-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: Album
---

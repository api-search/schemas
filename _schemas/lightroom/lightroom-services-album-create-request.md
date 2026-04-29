---
description: ''
layout: schema
name: AlbumCreateRequest
properties_list:
- description: Album subtype
  name: subtype
  type: string
- description: ''
  name: payload
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-services-album-create-request-schema.json
slug: lightroom-services-album-create-request
source_filename: lightroom-services-album-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlbumCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"Album subtype\"\n    },\n    \"payload\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-services-album-create-request-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: AlbumCreateRequest
---

---
description: ''
layout: schema
name: AlbumsListResponse
properties_list:
- description: ''
  name: base
  type: string
- description: List of album resources
  name: resources
  type: array
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-services-albums-list-response-schema.json
slug: lightroom-services-albums-list-response
source_filename: lightroom-services-albums-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlbumsListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base\": {\n      \"type\": \"string\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"List of album resources\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-services-albums-list-response-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: AlbumsListResponse
---

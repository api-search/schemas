---
description: ''
layout: schema
name: AlbumAssetsRequest
properties_list:
- description: List of asset references to add to the album
  name: resources
  type: array
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-services-album-assets-request-schema.json
slug: lightroom-services-album-assets-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlbumAssetsRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"List of asset references to add to the album\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-services-album-assets-request-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: AlbumAssetsRequest
---

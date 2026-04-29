---
description: ''
layout: schema
name: AssetsListResponse
properties_list:
- description: Base URL for the API
  name: base
  type: string
- description: List of asset resources
  name: resources
  type: array
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-services-assets-list-response-schema.json
slug: lightroom-services-assets-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetsListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base\": {\n      \"type\": \"string\",\n      \"description\": \"Base URL for the API\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"List of asset resources\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-services-assets-list-response-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: AssetsListResponse
---

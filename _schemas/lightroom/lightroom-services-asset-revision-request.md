---
description: ''
layout: schema
name: AssetRevisionRequest
properties_list:
- description: Asset subtype
  name: subtype
  type: string
- description: Asset metadata payload
  name: payload
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-services-asset-revision-request-schema.json
slug: lightroom-services-asset-revision-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetRevisionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"Asset subtype\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Asset metadata payload\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-services-asset-revision-request-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: AssetRevisionRequest
---

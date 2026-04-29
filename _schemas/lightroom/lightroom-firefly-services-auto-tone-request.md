---
description: ''
layout: schema
name: AutoToneRequest
properties_list:
- description: ''
  name: inputs
  type: object
- description: One or more output destinations
  name: outputs
  type: array
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-firefly-services-auto-tone-request-schema.json
slug: lightroom-firefly-services-auto-tone-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutoToneRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"object\"\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"One or more output destinations\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-firefly-services-auto-tone-request-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: AutoToneRequest
---

---
description: ''
layout: schema
name: SpaceRequest
properties_list:
- description: Space name
  name: name
  type: string
- description: Space visibility
  name: visibility
  type: string
- description: Space description
  name: description
  type: string
provider_name: Archbee
provider_slug: archbee
schema_file: json-schema/archbee-api-space-request-schema.json
slug: archbee-api-space-request
source_filename: archbee-api-space-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Space name\",\n      \"example\": \"API Reference\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Space visibility\",\n      \"enum\": [\n        \"public\",\n        \"private\",\n        \"password-protected\"\n      ],\n      \"example\": \"public\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Space description\",\n      \"example\": \"API reference documentation\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-space-request-schema.json\",\n  \"title\": \"SpaceRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-space-request-schema.json
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
title: SpaceRequest
---

---
description: ''
layout: schema
name: Space
properties_list:
- description: Unique space identifier
  name: id
  type: string
- description: Space display name
  name: name
  type: string
- description: URL-friendly space identifier
  name: slug
  type: string
- description: Space visibility
  name: visibility
  type: string
- description: Space description
  name: description
  type: string
- description: Number of pages in the space
  name: pageCount
  type: integer
- description: Space creation timestamp
  name: createdAt
  type: string
provider_name: Archbee
provider_slug: archbee
schema_file: json-schema/archbee-api-space-schema.json
slug: archbee-api-space
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique space identifier\",\n      \"example\": \"sp_abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Space display name\",\n      \"example\": \"Developer Docs\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly space identifier\",\n      \"example\": \"developer-docs\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Space visibility\",\n      \"enum\": [\n        \"public\",\n        \"private\",\n        \"password-protected\"\n      ],\n      \"example\": \"public\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Space description\",\n      \"example\": \"Main developer documentation\"\n    },\n    \"pageCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pages in the space\"\
  ,\n      \"example\": 42\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Space creation timestamp\",\n      \"example\": \"2026-01-15T10:00:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-space-schema.json\",\n  \"title\": \"Space\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-space-schema.json
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
title: Space
---

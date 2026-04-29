---
description: ''
layout: schema
name: Page
properties_list:
- description: Unique page identifier
  name: id
  type: string
- description: Page title
  name: title
  type: string
- description: URL-friendly page identifier
  name: slug
  type: string
- description: Page publication status
  name: status
  type: string
- description: Page content in Markdown
  name: content
  type: string
- description: Parent space identifier
  name: spaceId
  type: string
- description: Parent page identifier (if nested)
  name: parentId
  type: string
- description: Last update timestamp
  name: updatedAt
  type: string
provider_name: Archbee
provider_slug: archbee
schema_file: json-schema/archbee-api-page-schema.json
slug: archbee-api-page
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique page identifier\",\n      \"example\": \"pg_abc123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Page title\",\n      \"example\": \"Getting Started\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly page identifier\",\n      \"example\": \"getting-started\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Page publication status\",\n      \"enum\": [\n        \"draft\",\n        \"published\",\n        \"archived\"\n      ],\n      \"example\": \"published\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Page content in Markdown\",\n      \"example\": \"# Getting Started\\n\\nWelcome to our API...\"\n    },\n    \"spaceId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent space identifier\"\
  ,\n      \"example\": \"sp_abc123\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent page identifier (if nested)\",\n      \"example\": \"pg_parent123\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-page-schema.json\",\n  \"title\": \"Page\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-page-schema.json
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
title: Page
---

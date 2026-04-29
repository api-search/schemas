---
description: ''
layout: schema
name: PageRequest
properties_list:
- description: Page title
  name: title
  type: string
- description: Page content in Markdown
  name: content
  type: string
- description: Page status
  name: status
  type: string
- description: Parent page ID for nested pages
  name: parentId
  type: string
provider_name: Archbee
provider_slug: archbee
schema_file: json-schema/archbee-api-page-request-schema.json
slug: archbee-api-page-request
source_filename: archbee-api-page-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"title\"\n  ],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Page title\",\n      \"example\": \"Quick Start Guide\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Page content in Markdown\",\n      \"example\": \"# Quick Start\\n\\nWelcome to our API...\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Page status\",\n      \"enum\": [\n        \"draft\",\n        \"published\"\n      ],\n      \"example\": \"draft\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent page ID for nested pages\",\n      \"example\": \"pg_parent123\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-page-request-schema.json\",\n  \"title\": \"PageRequest\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/json-schema/archbee-api-page-request-schema.json
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
title: PageRequest
---

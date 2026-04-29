---
description: Cursor-based pagination metadata.
layout: schema
name: Pagination
properties_list:
- description: Cursor value for the page before the current one.
  name: before
  type: number
- description: Cursor value for the page after the current one.
  name: after
  type: number
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-pagination-schema.json
slug: figma-rest-pagination
source_filename: figma-rest-pagination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Pagination\",\n  \"type\": \"object\",\n  \"description\": \"Cursor-based pagination metadata.\",\n  \"properties\": {\n    \"before\": {\n      \"type\": \"number\",\n      \"description\": \"Cursor value for the page before the current one.\"\n    },\n    \"after\": {\n      \"type\": \"number\",\n      \"description\": \"Cursor value for the page after the current one.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-pagination-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Pagination
---

---
description: ''
layout: schema
name: PaginationMeta
properties_list:
- description: Total number of results available.
  name: results
  type: integer
- description: Number of results per page.
  name: limit
  type: integer
- description: Current offset position.
  name: offset
  type: integer
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-pagination-meta-schema.json
slug: hunter-pagination-meta
source_filename: hunter-pagination-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginationMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of results available.\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results per page.\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Current offset position.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-pagination-meta-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: PaginationMeta
---

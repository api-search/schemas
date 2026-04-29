---
description: Pagination links for list responses following JSON:API specification.
layout: schema
name: Pagination
properties_list:
- description: URL of the first page.
  name: first
  type: string
- description: URL of the last page.
  name: last
  type: string
- description: URL of the previous page, or null.
  name: prev
  type: string
- description: URL of the next page, or null.
  name: next
  type: string
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-pagination-schema.json
slug: better-stack-pagination
source_filename: better-stack-pagination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-pagination-schema.json\",\n  \"title\": \"Pagination\",\n  \"description\": \"Pagination links for list responses following JSON:API specification.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the first page.\",\n      \"example\": \"https://uptime.betterstack.com/api/v2/monitors?page=1\"\n    },\n    \"last\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the last page.\",\n      \"example\": \"https://uptime.betterstack.com/api/v2/monitors?page=5\"\n    },\n    \"prev\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"nullable\": true,\n      \"description\": \"URL of the previous page, or null.\",\n      \"example\"\
  : null\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"nullable\": true,\n      \"description\": \"URL of the next page, or null.\",\n      \"example\": \"https://uptime.betterstack.com/api/v2/monitors?page=2\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-pagination-schema.json
tags:
- Incidents
- Logs
- Monitoring
- Platform
- Status
- Uptime
- Observability
- On-Call
- Heartbeats
title: Pagination
---

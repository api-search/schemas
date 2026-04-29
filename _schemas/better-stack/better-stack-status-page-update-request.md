---
description: Request body for updating a status page (all fields optional).
layout: schema
name: StatusPageUpdateRequest
properties_list:
- description: New company name.
  name: company_name
  type: string
- description: New custom domain.
  name: custom_domain
  type: string
- description: New theme.
  name: theme
  type: string
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-status-page-update-request-schema.json
slug: better-stack-status-page-update-request
source_filename: better-stack-status-page-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-status-page-update-request-schema.json\",\n  \"title\": \"StatusPageUpdateRequest\",\n  \"description\": \"Request body for updating a status page (all fields optional).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"New company name.\",\n      \"example\": \"Acme Corp Updated\"\n    },\n    \"custom_domain\": {\n      \"type\": \"string\",\n      \"description\": \"New custom domain.\",\n      \"example\": \"status.acme.com\"\n    },\n    \"theme\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"light\",\n        \"dark\"\n      ],\n      \"description\": \"New theme.\",\n      \"example\": \"dark\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-status-page-update-request-schema.json
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
title: StatusPageUpdateRequest
---

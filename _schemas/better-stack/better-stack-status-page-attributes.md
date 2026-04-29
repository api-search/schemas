---
description: Attributes of a status page.
layout: schema
name: StatusPageAttributes
properties_list:
- description: Name of the company displayed on the status page.
  name: company_name
  type: string
- description: URL of the company website.
  name: company_website
  type: string
- description: Subdomain for the status page (yourname.betteruptime.com).
  name: subdomain
  type: string
- description: Custom domain for the status page.
  name: custom_domain
  type: string
- description: Timezone for the status page.
  name: timezone
  type: string
- description: UI theme for the status page.
  name: theme
  type: string
- description: Overall operational state across all monitored resources.
  name: aggregate_state
  type: string
- description: When the status page was created.
  name: created_at
  type: string
- description: When the status page was last updated.
  name: updated_at
  type: string
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-status-page-attributes-schema.json
slug: better-stack-status-page-attributes
source_filename: better-stack-status-page-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-status-page-attributes-schema.json\",\n  \"title\": \"StatusPageAttributes\",\n  \"description\": \"Attributes of a status page.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the company displayed on the status page.\",\n      \"example\": \"Acme Corp\"\n    },\n    \"company_website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the company website.\",\n      \"example\": \"https://acme.com\"\n    },\n    \"subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Subdomain for the status page (yourname.betteruptime.com).\",\n      \"example\": \"acme\"\n    },\n    \"custom_domain\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n\
  \      \"description\": \"Custom domain for the status page.\",\n      \"example\": \"status.acme.com\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for the status page.\",\n      \"example\": \"UTC\"\n    },\n    \"theme\": {\n      \"type\": \"string\",\n      \"description\": \"UI theme for the status page.\",\n      \"enum\": [\n        \"light\",\n        \"dark\"\n      ],\n      \"example\": \"light\"\n    },\n    \"aggregate_state\": {\n      \"type\": \"string\",\n      \"description\": \"Overall operational state across all monitored resources.\",\n      \"enum\": [\n        \"operational\",\n        \"degraded_performance\",\n        \"partial_outage\",\n        \"major_outage\",\n        \"maintenance\",\n        \"downtime\"\n      ],\n      \"example\": \"operational\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the status page was created.\",\n\
  \      \"example\": \"2025-03-01T00:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the status page was last updated.\",\n      \"example\": \"2026-04-01T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-status-page-attributes-schema.json
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
title: StatusPageAttributes
---

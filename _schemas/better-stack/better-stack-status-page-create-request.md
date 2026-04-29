---
description: Request body for creating a status page.
layout: schema
name: StatusPageCreateRequest
properties_list:
- description: Company name displayed on the page.
  name: company_name
  type: string
- description: Company website URL.
  name: company_website
  type: string
- description: Subdomain slug.
  name: subdomain
  type: string
- description: Timezone for the page.
  name: timezone
  type: string
- description: Page theme.
  name: theme
  type: string
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-status-page-create-request-schema.json
slug: better-stack-status-page-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-status-page-create-request-schema.json\",\n  \"title\": \"StatusPageCreateRequest\",\n  \"description\": \"Request body for creating a status page.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Company name displayed on the page.\",\n      \"example\": \"Acme Corp\"\n    },\n    \"company_website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Company website URL.\",\n      \"example\": \"https://acme.com\"\n    },\n    \"subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Subdomain slug.\",\n      \"example\": \"acme\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for the page.\",\n      \"example\": \"UTC\"\
  \n    },\n    \"theme\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"light\",\n        \"dark\"\n      ],\n      \"description\": \"Page theme.\",\n      \"example\": \"light\"\n    }\n  },\n  \"required\": [\n    \"company_name\",\n    \"subdomain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-status-page-create-request-schema.json
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
title: StatusPageCreateRequest
---

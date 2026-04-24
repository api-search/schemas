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

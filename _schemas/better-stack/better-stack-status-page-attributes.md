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

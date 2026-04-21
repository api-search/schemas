---
description: HealthStatus schema from ARGUS Enterprise API
layout: schema
name: HealthStatus
properties_list:
- description: Overall service health
  name: status
  type: string
- description: Number of events pending delivery
  name: queueDepth
  type: integer
- description: Error rate over the last hour (percentage)
  name: recentErrorRate
  type: number
- description: Service uptime duration
  name: uptime
  type: string
- description: Timestamp of last health check
  name: lastChecked
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-health-status-schema.json
slug: argus-enterprise-health-status
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: HealthStatus
---

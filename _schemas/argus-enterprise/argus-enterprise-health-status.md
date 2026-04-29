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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-health-status-schema.json\",\n  \"title\": \"HealthStatus\",\n  \"description\": \"HealthStatus schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Healthy\",\n        \"Degraded\",\n        \"Unhealthy\"\n      ],\n      \"description\": \"Overall service health\"\n    },\n    \"queueDepth\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of events pending delivery\"\n    },\n    \"recentErrorRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Error rate over the last hour (percentage)\"\n    },\n    \"uptime\": {\n      \"type\": \"string\",\n      \"description\": \"Service uptime duration\"\n    },\n    \"lastChecked\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last health check\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-health-status-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: HealthStatus
---

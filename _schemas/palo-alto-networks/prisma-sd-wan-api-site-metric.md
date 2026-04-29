---
description: SiteMetric schema from Palo Alto Networks Prisma SD-WAN API
layout: schema
name: SiteMetric
properties_list:
- description: Time bucket for the aggregated metric.
  name: timestamp
  type: string
- description: Site identifier.
  name: site_id
  type: string
- description: WAN interface name.
  name: interface_name
  type: string
- description: Type of metric.
  name: metric_type
  type: string
- description: Metric value.
  name: value
  type: number
- description: Unit of measurement (e.g., Mbps, ms, pct).
  name: unit
  type: string
- description: Traffic direction for bandwidth metrics.
  name: direction
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-sd-wan-api-site-metric-schema.json
slug: prisma-sd-wan-api-site-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SiteMetric\",\n  \"description\": \"SiteMetric schema from Palo Alto Networks Prisma SD-WAN API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-site-metric-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time bucket for the aggregated metric.\"\n    },\n    \"site_id\": {\n      \"type\": \"string\",\n      \"description\": \"Site identifier.\"\n    },\n    \"interface_name\": {\n      \"type\": \"string\",\n      \"description\": \"WAN interface name.\"\n    },\n    \"metric_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"bandwidth\",\n        \"latency\",\n        \"jitter\",\n        \"packet_loss\"\n      ],\n      \"description\": \"Type of metric.\"\n    },\n  \
  \  \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Metric value.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement (e.g., Mbps, ms, pct).\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"upload\",\n        \"download\"\n      ],\n      \"description\": \"Traffic direction for bandwidth metrics.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-site-metric-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SiteMetric
---

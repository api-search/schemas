---
description: PerformanceMetric schema from Palo Alto Networks Autonomous DEM API
layout: schema
name: PerformanceMetric
properties_list:
- description: Time bucket for the aggregated metric.
  name: timestamp
  type: string
- description: User identifier.
  name: user_id
  type: string
- description: Site name.
  name: site_name
  type: string
- description: Application identifier if metric is application-specific.
  name: app_id
  type: string
- description: Type of performance metric.
  name: metric_type
  type: string
- description: Metric value in the appropriate unit for the metric type.
  name: value
  type: number
- description: Unit of measurement (e.g., ms, pct, Mbps).
  name: unit
  type: string
- description: Network segment this metric applies to.
  name: segment
  type: string
- description: Number of measurement samples in this time bucket.
  name: sample_count
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/autonomous-dem-api-performance-metric-schema.json
slug: autonomous-dem-api-performance-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PerformanceMetric\",\n  \"description\": \"PerformanceMetric schema from Palo Alto Networks Autonomous DEM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-performance-metric-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time bucket for the aggregated metric.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier.\"\n    },\n    \"site_name\": {\n      \"type\": \"string\",\n      \"description\": \"Site name.\"\n    },\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"Application identifier if metric is application-specific.\"\n    },\n    \"metric_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n     \
  \   \"latency\",\n        \"packet_loss\",\n        \"jitter\",\n        \"throughput\",\n        \"dns_resolution\",\n        \"tcp_connection\"\n      ],\n      \"description\": \"Type of performance metric.\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Metric value in the appropriate unit for the metric type.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement (e.g., ms, pct, Mbps).\"\n    },\n    \"segment\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"endpoint\",\n        \"local_network\",\n        \"isp\",\n        \"prisma_access\",\n        \"application\"\n      ],\n      \"description\": \"Network segment this metric applies to.\"\n    },\n    \"sample_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of measurement samples in this time bucket.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-performance-metric-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PerformanceMetric
---

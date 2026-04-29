---
description: NetworkMetrics schema
layout: schema
name: NetworkMetrics
properties_list:
- description: Current network generation for the device
  name: networkGeneration
  type: string
- description: Signal quality indicator
  name: signalStrength
  type: string
- description: Estimated downlink throughput in Mbps
  name: estimatedDownlinkThroughput
  type: integer
- description: Estimated uplink throughput in Mbps
  name: estimatedUplinkThroughput
  type: integer
- description: Estimated round-trip latency in milliseconds
  name: estimatedLatency
  type: integer
- description: Current network congestion level
  name: congestionLevel
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/network-insights-api-network-metrics-schema.json
slug: network-insights-api-network-metrics
source_filename: network-insights-api-network-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/network-insights-api-network-metrics-schema.json\",\n  \"title\": \"NetworkMetrics\",\n  \"description\": \"NetworkMetrics schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkGeneration\": {\n      \"type\": \"string\",\n      \"description\": \"Current network generation for the device\",\n      \"enum\": [\n        \"5G\",\n        \"5G_NSA\",\n        \"4G\",\n        \"3G\"\n      ],\n      \"example\": \"5G\"\n    },\n    \"signalStrength\": {\n      \"type\": \"string\",\n      \"description\": \"Signal quality indicator\",\n      \"enum\": [\n        \"EXCELLENT\",\n        \"GOOD\",\n        \"FAIR\",\n        \"POOR\"\n      ],\n      \"example\": \"GOOD\"\n    },\n    \"estimatedDownlinkThroughput\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated downlink\
  \ throughput in Mbps\",\n      \"example\": 250\n    },\n    \"estimatedUplinkThroughput\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated uplink throughput in Mbps\",\n      \"example\": 50\n    },\n    \"estimatedLatency\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated round-trip latency in milliseconds\",\n      \"example\": 15\n    },\n    \"congestionLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Current network congestion level\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\"\n      ],\n      \"example\": \"LOW\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/network-insights-api-network-metrics-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: NetworkMetrics
---

---
description: Network performance metrics for a device on AT&T network
layout: schema
name: Network Metrics
properties_list:
- description: ''
  name: networkGeneration
  type: string
- description: ''
  name: signalStrength
  type: string
- description: ''
  name: estimatedDownlinkThroughput
  type: number
- description: ''
  name: estimatedLatency
  type: integer
- description: ''
  name: congestionLevel
  type: string
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/network-apis-network-metrics-schema.json
slug: network-apis-network-metrics
source_filename: network-apis-network-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/network/network-metrics\",\n  \"title\": \"Network Metrics\",\n  \"description\": \"Network performance metrics for a device on AT&T network\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkGeneration\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"5G\",\n        \"5G_NSA\",\n        \"4G\",\n        \"3G\"\n      ]\n    },\n    \"signalStrength\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"EXCELLENT\",\n        \"GOOD\",\n        \"FAIR\",\n        \"POOR\"\n      ]\n    },\n    \"estimatedDownlinkThroughput\": {\n      \"type\": \"number\",\n      \"format\": \"float\"\n    },\n    \"estimatedLatency\": {\n      \"type\": \"integer\"\n    },\n    \"congestionLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/network-apis-network-metrics-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Network Metrics
---

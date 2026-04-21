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

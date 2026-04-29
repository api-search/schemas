---
description: NetworkMetricsRequest schema
layout: schema
name: NetworkMetricsRequest
properties_list:
- description: Device identifier for network metrics queries
  name: device
  type: object
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/network-insights-api-network-metrics-request-schema.json
slug: network-insights-api-network-metrics-request
source_filename: network-insights-api-network-metrics-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/network-insights-api-network-metrics-request-schema.json\",\n  \"title\": \"NetworkMetricsRequest\",\n  \"description\": \"NetworkMetricsRequest schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"device\"\n  ],\n  \"properties\": {\n    \"device\": {\n      \"type\": \"object\",\n      \"description\": \"Device identifier for network metrics queries\",\n      \"properties\": {\n        \"phoneNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Mobile phone number in E.164 format\",\n          \"example\": \"+12125551234\"\n        },\n        \"ipv4Address\": {\n          \"type\": \"object\",\n          \"description\": \"Device IP address (alternative to phoneNumber)\",\n          \"properties\": {\n            \"publicAddress\": {\n              \"type\": \"string\"\
  ,\n              \"example\": \"203.0.113.42\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/network-insights-api-network-metrics-request-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: NetworkMetricsRequest
---

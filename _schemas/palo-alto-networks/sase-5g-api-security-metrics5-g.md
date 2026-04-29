---
description: SecurityMetrics5G schema from Palo Alto Networks SASE 5G Managed Services API
layout: schema
name: SecurityMetrics5G
properties_list:
- description: ''
  name: period
  type: object
- description: Total 5G sessions inspected during the period.
  name: total_sessions
  type: integer
- description: Number of threats detected in 5G traffic.
  name: threats_detected
  type: integer
- description: Number of threats blocked.
  name: threats_blocked
  type: integer
- description: Total bytes of 5G traffic inspected.
  name: bytes_inspected
  type: integer
- description: Number of active 5G subscribers.
  name: active_subscribers
  type: integer
- description: Metrics broken down by network slice.
  name: per_slice_metrics
  type: array
- description: Time-series data points for the metrics period.
  name: time_series
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-api-security-metrics5-g-schema.json
slug: sase-5g-api-security-metrics5-g
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityMetrics5G\",\n  \"description\": \"SecurityMetrics5G schema from Palo Alto Networks SASE 5G Managed Services API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-security-metrics5-g-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"period\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"total_sessions\": {\n      \"type\": \"integer\",\n      \"description\": \"Total 5G sessions inspected during the period.\"\n    },\n    \"threats_detected\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of threats detected in 5G traffic.\"\n    },\n   \
  \ \"threats_blocked\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of threats blocked.\"\n    },\n    \"bytes_inspected\": {\n      \"type\": \"integer\",\n      \"description\": \"Total bytes of 5G traffic inspected.\"\n    },\n    \"active_subscribers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active 5G subscribers.\"\n    },\n    \"per_slice_metrics\": {\n      \"type\": \"array\",\n      \"description\": \"Metrics broken down by network slice.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"slice_id\": {\n            \"type\": \"string\"\n          },\n          \"slice_name\": {\n            \"type\": \"string\"\n          },\n          \"sessions\": {\n            \"type\": \"integer\"\n          },\n          \"threats_detected\": {\n            \"type\": \"integer\"\n          },\n          \"bytes_inspected\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n  \
  \  },\n    \"time_series\": {\n      \"type\": \"array\",\n      \"description\": \"Time-series data points for the metrics period.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"sessions\": {\n            \"type\": \"integer\"\n          },\n          \"threats\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-security-metrics5-g-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SecurityMetrics5G
---

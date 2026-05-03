---
description: Describes a connected store endpoint in Thanos, including its type, available time range, external labels, and health status.
layout: schema
name: Thanos Store Info
properties_list:
- description: Address or identifier of the store endpoint (e.g., sidecar gRPC address).
  name: name
  type: string
- description: The type of Thanos store component.
  name: storeType
  type: string
- description: External label sets advertised by this store, used for identifying data origin and deduplication.
  name: labelSets
  type: array
- description: Minimum timestamp in milliseconds since epoch for data available from this store.
  name: minTime
  type: integer
- description: Maximum timestamp in milliseconds since epoch for data available from this store.
  name: maxTime
  type: integer
- description: ISO 8601 timestamp of the last successful health check.
  name: lastCheck
  type: string
- description: Last error message from this store, or null if the store is healthy.
  name: lastError
  type:
  - string
  - 'null'
provider_name: Thanos
provider_slug: thanos
schema_file: json-schema/store-info.json
slug: store-info
source_filename: store-info.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://thanos.io/schemas/store-info.json\",\n  \"title\": \"Thanos Store Info\",\n  \"description\": \"Describes a connected store endpoint in Thanos, including its type, available time range, external labels, and health status.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"storeType\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Address or identifier of the store endpoint (e.g., sidecar gRPC address).\"\n    },\n    \"storeType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of Thanos store component.\",\n      \"enum\": [\n        \"sidecar\",\n        \"store\",\n        \"rule\",\n        \"receive\",\n        \"debug\",\n        \"unknown\"\n      ]\n    },\n    \"labelSets\": {\n      \"type\": \"array\",\n      \"description\": \"External label sets advertised by this store, used for identifying\
  \ data origin and deduplication.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"minTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Minimum timestamp in milliseconds since epoch for data available from this store.\"\n    },\n    \"maxTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Maximum timestamp in milliseconds since epoch for data available from this store.\"\n    },\n    \"lastCheck\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last successful health check.\"\n    },\n    \"lastError\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"description\": \"Last error message from this store, or null if the store is healthy.\"\n    }\n  },\n  \"examples\": [\n    {\n      \"name\":\
  \ \"sidecar-prometheus-0:10901\",\n      \"storeType\": \"sidecar\",\n      \"labelSets\": [\n        {\n          \"cluster\": \"us-east-1\",\n          \"prometheus\": \"monitoring/prometheus-0\"\n        }\n      ],\n      \"minTime\": 1672531200000,\n      \"maxTime\": 1704067200000,\n      \"lastCheck\": \"2025-06-15T12:00:00Z\",\n      \"lastError\": null\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/thanos/refs/heads/main/json-schema/store-info.json
tags:
- Metrics
- Monitoring
- Observability
- Prometheus
- Time Series Database
title: Thanos Store Info
---

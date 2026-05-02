---
description: A multicluster gateway entry with alive status, paired service count, and latency metrics.
layout: schema
name: Linkerd Gateway
properties_list:
- description: Kubernetes namespace of the gateway.
  name: namespace
  type: string
- description: Name of the gateway.
  name: name
  type: string
- description: Name of the remote cluster.
  name: cluster_name
  type: string
- description: Number of services paired through this gateway.
  name: paired_services
  type: integer
- description: Whether the gateway is currently alive and reachable.
  name: alive
  type: boolean
- description: 50th percentile latency in milliseconds.
  name: latency_ms_p50
  type: number
- description: 95th percentile latency in milliseconds.
  name: latency_ms_p95
  type: number
- description: 99th percentile latency in milliseconds.
  name: latency_ms_p99
  type: number
provider_name: Linkerd
provider_slug: linkerd
schema_file: json-schema/gateway.json
slug: gateway
source_filename: gateway.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/linkerd/blob/main/json-schema/gateway.json\",\n  \"title\": \"Linkerd Gateway\",\n  \"description\": \"A multicluster gateway entry with alive status, paired service count, and latency metrics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes namespace of the gateway.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the gateway.\"\n    },\n    \"cluster_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the remote cluster.\"\n    },\n    \"paired_services\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of services paired through this gateway.\"\n    },\n    \"alive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the gateway is currently alive and reachable.\"\n    },\n  \
  \  \"latency_ms_p50\": {\n      \"type\": \"number\",\n      \"description\": \"50th percentile latency in milliseconds.\"\n    },\n    \"latency_ms_p95\": {\n      \"type\": \"number\",\n      \"description\": \"95th percentile latency in milliseconds.\"\n    },\n    \"latency_ms_p99\": {\n      \"type\": \"number\",\n      \"description\": \"99th percentile latency in milliseconds.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/json-schema/gateway.json
tags:
- Kubernetes
- mTLS
- Observability
- Security
- Service Mesh
title: Linkerd Gateway
---

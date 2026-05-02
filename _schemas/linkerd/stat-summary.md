---
description: Aggregated golden metrics for a Kubernetes resource including request rate, success rate, and latency percentiles as returned by the Linkerd Viz Metrics API.
layout: schema
name: Linkerd Stat Summary
properties_list:
- description: Successful response containing stat tables.
  name: ok
  type: object
- description: Error response.
  name: error
  type: object
provider_name: Linkerd
provider_slug: linkerd
schema_file: json-schema/stat-summary.json
slug: stat-summary
source_filename: stat-summary.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/linkerd/blob/main/json-schema/stat-summary.json\",\n  \"title\": \"Linkerd Stat Summary\",\n  \"description\": \"Aggregated golden metrics for a Kubernetes resource including request rate, success rate, and latency percentiles as returned by the Linkerd Viz Metrics API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ok\": {\n      \"type\": \"object\",\n      \"description\": \"Successful response containing stat tables.\",\n      \"properties\": {\n        \"stat_tables\": {\n          \"type\": \"array\",\n          \"description\": \"Array of stat tables grouped by pod group.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/StatTable\"\n          }\n        }\n      }\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Error response.\",\n      \"properties\": {\n        \"error\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Error message.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"StatTable\": {\n      \"type\": \"object\",\n      \"description\": \"A table of stat rows grouped by pod group.\",\n      \"properties\": {\n        \"pod_group\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"rows\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/$defs/StatTableRow\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"StatTableRow\": {\n      \"type\": \"object\",\n      \"description\": \"A single row of metrics for a Kubernetes resource.\",\n      \"properties\": {\n        \"resource\": {\n          \"$ref\": \"#/$defs/Resource\"\n        },\n        \"time_window\": {\n          \"type\": \"string\",\n          \"description\": \"Time window for the aggregated metrics.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Status of the resource.\"\n        },\n        \"meshed_pod_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of pods in the mesh.\"\n        },\n        \"running_pod_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of running pods.\"\n        },\n        \"failed_pod_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of failed pods.\"\n        },\n        \"stats\": {\n          \"$ref\": \"#/$defs/BasicStats\"\n        },\n        \"tcp_stats\": {\n          \"$ref\": \"#/$defs/TcpStats\"\n        }\n      }\n    },\n    \"BasicStats\": {\n      \"type\": \"object\",\n      \"description\": \"Golden metrics for request traffic.\",\n      \"properties\": {\n        \"success_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of successful requests.\"\n        },\n        \"failure_count\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Number of failed requests.\"\n        },\n        \"latency_ms_p50\": {\n          \"type\": \"number\",\n          \"description\": \"50th percentile latency in milliseconds.\"\n        },\n        \"latency_ms_p95\": {\n          \"type\": \"number\",\n          \"description\": \"95th percentile latency in milliseconds.\"\n        },\n        \"latency_ms_p99\": {\n          \"type\": \"number\",\n          \"description\": \"99th percentile latency in milliseconds.\"\n        },\n        \"actual_success_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Actual number of successful requests (before retries).\"\n        },\n        \"actual_failure_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Actual number of failed requests (before retries).\"\n        }\n      }\n    },\n    \"TcpStats\": {\n      \"type\": \"object\",\n      \"description\": \"TCP-level connection statistics.\",\n      \"properties\": {\n        \"open_connections\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Number of currently open TCP connections.\"\n        },\n        \"read_bytes_total\": {\n          \"type\": \"integer\",\n          \"description\": \"Total bytes read.\"\n        },\n        \"write_bytes_total\": {\n          \"type\": \"integer\",\n          \"description\": \"Total bytes written.\"\n        }\n      }\n    },\n    \"Resource\": {\n      \"type\": \"object\",\n      \"description\": \"A Kubernetes resource reference.\",\n      \"properties\": {\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes namespace.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Resource type (e.g., deployment, pod, service).\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/json-schema/stat-summary.json
tags:
- Kubernetes
- mTLS
- Observability
- Security
- Service Mesh
title: Linkerd Stat Summary
---

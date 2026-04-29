---
description: Strategy for retrying failed steps
layout: schema
name: RetryStrategy
properties_list:
- description: Maximum number of retries
  name: limit
  type: integer
- description: ''
  name: retryPolicy
  type: string
- description: ''
  name: backoff
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-retry-strategy-schema.json
slug: argo-workflows-retry-strategy
source_filename: argo-workflows-retry-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-retry-strategy-schema.json\",\n  \"title\": \"RetryStrategy\",\n  \"description\": \"Strategy for retrying failed steps\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of retries\"\n    },\n    \"retryPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Always\",\n        \"OnFailure\",\n        \"OnError\",\n        \"OnTransientError\"\n      ]\n    },\n    \"backoff\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"duration\": {\n          \"type\": \"string\"\n        },\n        \"factor\": {\n          \"type\": \"integer\"\n        },\n        \"maxDuration\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-retry-strategy-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: RetryStrategy
---

---
description: v1alpha1RetryStrategy schema from Argo CD API
layout: schema
name: v1alpha1RetryStrategy
properties_list:
- description: ''
  name: backoff
  type: object
- description: Limit is the maximum number of attempts for retrying a failed sync. If set to 0, no retries will be performed.
  name: limit
  type: integer
- description: ''
  name: refresh
  type: boolean
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-retry-strategy-schema.json
slug: argo-cd-v1alpha1-retry-strategy
source_filename: argo-cd-v1alpha1-retry-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-retry-strategy-schema.json\",\n  \"title\": \"v1alpha1RetryStrategy\",\n  \"description\": \"v1alpha1RetryStrategy schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"backoff\": {\n      \"$ref\": \"#/definitions/v1alpha1Backoff\"\n    },\n    \"limit\": {\n      \"description\": \"Limit is the maximum number of attempts for retrying a failed sync. If set to 0, no retries will be performed.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"refresh\": {\n      \"type\": \"boolean\",\n      \"title\": \"Refresh indicates if the latest revision should be used on retry instead of the initial one (default: false)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-retry-strategy-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1RetryStrategy
---

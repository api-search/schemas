---
description: v1alpha1Backoff schema from Argo CD API
layout: schema
name: v1alpha1Backoff
properties_list:
- description: ''
  name: duration
  type: string
- description: ''
  name: factor
  type: integer
- description: ''
  name: maxDuration
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-backoff-schema.json
slug: argo-cd-v1alpha1-backoff
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-backoff-schema.json\",\n  \"title\": \"v1alpha1Backoff\",\n  \"description\": \"v1alpha1Backoff schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"type\": \"string\",\n      \"title\": \"Duration is the amount to back off. Default unit is seconds, but could also be a duration (e.g. \\\"2m\\\", \\\"1h\\\")\"\n    },\n    \"factor\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"Factor is a factor to multiply the base duration after each failed retry\"\n    },\n    \"maxDuration\": {\n      \"type\": \"string\",\n      \"title\": \"MaxDuration is the maximum amount of time allowed for the backoff strategy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-backoff-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1Backoff
---

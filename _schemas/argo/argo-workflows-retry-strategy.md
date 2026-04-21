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

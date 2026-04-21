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

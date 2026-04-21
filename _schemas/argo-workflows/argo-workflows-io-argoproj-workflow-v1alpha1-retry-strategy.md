---
description: RetryStrategy provides controls on how to retry a workflow step
layout: schema
name: io.argoproj.workflow.v1alpha1.RetryStrategy
properties_list:
- description: Affinity prevents running workflow's step on the same host
  name: affinity
  type: object
- description: Backoff is a backoff strategy
  name: backoff
  type: object
- description: Expression is a condition expression for when a node will be retried. If it evaluates to false, the node will not be retried and the retry strategy will be ignored
  name: expression
  type: string
- description: Limit is the maximum number of retry attempts when retrying a container. It does not include the original container; the maximum number of total attempts will be `limit + 1`.
  name: limit
  type: object
- description: RetryPolicy is a policy of NodePhase statuses that will be retried
  name: retryPolicy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-retry-strategy-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-retry-strategy
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.RetryStrategy
---

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
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-retry-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-retry-strategy-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.RetryStrategy\",\n  \"description\": \"RetryStrategy provides controls on how to retry a workflow step\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"affinity\": {\n      \"description\": \"Affinity prevents running workflow's step on the same host\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.RetryAffinity\"\n    },\n    \"backoff\": {\n      \"description\": \"Backoff is a backoff strategy\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Backoff\"\n    },\n    \"expression\": {\n      \"description\": \"Expression is a condition expression for when a node will be retried. If it evaluates to false, the node will not be retried and the retry\
  \ strategy will be ignored\",\n      \"type\": \"string\"\n    },\n    \"limit\": {\n      \"description\": \"Limit is the maximum number of retry attempts when retrying a container. It does not include the original container; the maximum number of total attempts will be `limit + 1`.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.util.intstr.IntOrString\"\n    },\n    \"retryPolicy\": {\n      \"description\": \"RetryPolicy is a policy of NodePhase statuses that will be retried\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-retry-strategy-schema.json
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

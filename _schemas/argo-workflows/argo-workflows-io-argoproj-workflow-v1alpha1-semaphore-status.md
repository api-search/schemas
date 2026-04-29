---
description: io.argoproj.workflow.v1alpha1.SemaphoreStatus schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.SemaphoreStatus
properties_list:
- description: Holding stores the list of resource acquired synchronization lock for workflows.
  name: holding
  type: array
- description: Waiting indicates the list of current synchronization lock holders.
  name: waiting
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-status-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.SemaphoreStatus\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.SemaphoreStatus schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"holding\": {\n      \"description\": \"Holding stores the list of resource acquired synchronization lock for workflows.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.SemaphoreHolding\"\n      }\n    },\n    \"waiting\": {\n      \"description\": \"Waiting indicates the list of current synchronization lock holders.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.SemaphoreHolding\"\
  \n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-status-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.SemaphoreStatus
---

---
description: Synchronization holds synchronization lock configuration
layout: schema
name: io.argoproj.workflow.v1alpha1.Synchronization
properties_list:
- description: 'v3.6 and after: Mutexes holds the list of Mutex lock details'
  name: mutexes
  type: array
- description: 'v3.6 and after: Semaphores holds the list of Semaphores configuration'
  name: semaphores
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-synchronization-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-synchronization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-synchronization-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.Synchronization\",\n  \"description\": \"Synchronization holds synchronization lock configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mutexes\": {\n      \"description\": \"v3.6 and after: Mutexes holds the list of Mutex lock details\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.Mutex\"\n      }\n    },\n    \"semaphores\": {\n      \"description\": \"v3.6 and after: Semaphores holds the list of Semaphores configuration\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.SemaphoreRef\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-synchronization-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Synchronization
---

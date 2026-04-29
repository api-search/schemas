---
description: SynchronizationStatus stores the status of semaphore and mutex.
layout: schema
name: io.argoproj.workflow.v1alpha1.SynchronizationStatus
properties_list:
- description: Mutex stores this workflow's mutex holder details
  name: mutex
  type: object
- description: Semaphore stores this workflow's Semaphore holder details
  name: semaphore
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-synchronization-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-synchronization-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-synchronization-status-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.SynchronizationStatus\",\n  \"description\": \"SynchronizationStatus stores the status of semaphore and mutex.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mutex\": {\n      \"description\": \"Mutex stores this workflow's mutex holder details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.MutexStatus\"\n    },\n    \"semaphore\": {\n      \"description\": \"Semaphore stores this workflow's Semaphore holder details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.SemaphoreStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-synchronization-status-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.SynchronizationStatus
---

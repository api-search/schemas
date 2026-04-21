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

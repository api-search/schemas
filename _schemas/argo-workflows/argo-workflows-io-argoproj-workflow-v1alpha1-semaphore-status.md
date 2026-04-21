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

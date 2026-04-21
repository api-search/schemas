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

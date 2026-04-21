---
description: SemaphoreRef is a reference of Semaphore
layout: schema
name: io.argoproj.workflow.v1alpha1.SemaphoreRef
properties_list:
- description: ConfigMapKeyRef is a configmap selector for Semaphore configuration
  name: configMapKeyRef
  type: object
- description: SyncDatabaseRef is a database reference for Semaphore configuration
  name: database
  type: object
- description: 'Namespace is the namespace of the configmap, default: [namespace of workflow]'
  name: namespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-ref-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-ref
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.SemaphoreRef
---

---
description: MutexStatus contains which objects hold mutex locks, and which objects this workflow is waiting on to release locks.
layout: schema
name: io.argoproj.workflow.v1alpha1.MutexStatus
properties_list:
- description: Holding is a list of mutexes and their respective objects that are held by mutex lock for this io.argoproj.workflow.v1alpha1.
  name: holding
  type: array
- description: Waiting is a list of mutexes and their respective objects this workflow is waiting for.
  name: waiting
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-status-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-mutex-status
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.MutexStatus
---

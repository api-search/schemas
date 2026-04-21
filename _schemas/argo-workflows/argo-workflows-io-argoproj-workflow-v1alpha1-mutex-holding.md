---
description: MutexHolding describes the mutex and the object which is holding it.
layout: schema
name: io.argoproj.workflow.v1alpha1.MutexHolding
properties_list:
- description: 'Holder is a reference to the object which holds the Mutex. Holding Scenario: 1. Current workflow''s NodeID which is holding the lock. e.g: ${NodeID} Waiting Scenario: 1. Current workflow or other workf'
  name: holder
  type: string
- description: 'Reference for the mutex e.g: ${namespace}/mutex/${mutexName}'
  name: mutex
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-holding-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-mutex-holding
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.MutexHolding
---

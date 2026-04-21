---
description: Mutex holds Mutex configuration
layout: schema
name: io.argoproj.workflow.v1alpha1.Mutex
properties_list:
- description: Database specifies this is database controlled if this is set true
  name: database
  type: boolean
- description: name of the mutex
  name: name
  type: string
- description: 'Namespace is the namespace of the mutex, default: [namespace of workflow]'
  name: namespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-mutex-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-mutex
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Mutex
---

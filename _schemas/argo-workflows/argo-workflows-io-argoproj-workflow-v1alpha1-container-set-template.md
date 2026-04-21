---
description: io.argoproj.workflow.v1alpha1.ContainerSetTemplate schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.ContainerSetTemplate
properties_list:
- description: ''
  name: containers
  type: array
- description: RetryStrategy describes how to retry container nodes if the container set fails. Note that this works differently from the template-level `retryStrategy` as it is a process-level retry that does not c
  name: retryStrategy
  type: object
- description: ''
  name: volumeMounts
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-container-set-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-container-set-template
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ContainerSetTemplate
---

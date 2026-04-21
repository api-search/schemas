---
description: ResourceFieldSelector represents container resources (cpu, memory) and their output format
layout: schema
name: io.k8s.api.core.v1.ResourceFieldSelector
properties_list:
- description: 'Container name: required for volumes, optional for env vars'
  name: containerName
  type: string
- description: Specifies the output format of the exposed resources, defaults to "1"
  name: divisor
  type: object
- description: 'Required: resource to select'
  name: resource
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-resource-field-selector-schema.json
slug: argo-workflows-io-k8s-api-core-v1-resource-field-selector
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ResourceFieldSelector
---

---
description: ContainerResizePolicy represents resource resize policy for the container.
layout: schema
name: io.k8s.api.core.v1.ContainerResizePolicy
properties_list:
- description: 'Name of the resource to which this resource resize policy applies. Supported values: cpu, memory.'
  name: resourceName
  type: string
- description: Restart policy to apply when specified resource is resized. If not specified, it defaults to NotRequired.
  name: restartPolicy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-container-resize-policy-schema.json
slug: argo-workflows-io-k8s-api-core-v1-container-resize-policy
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ContainerResizePolicy
---

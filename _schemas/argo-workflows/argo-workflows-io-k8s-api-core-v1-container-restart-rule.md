---
description: ContainerRestartRule describes how a container exit is handled.
layout: schema
name: io.k8s.api.core.v1.ContainerRestartRule
properties_list:
- description: Specifies the action taken on a container exit if the requirements are satisfied. The only possible value is "Restart" to restart the container.
  name: action
  type: string
- description: Represents the exit codes to check on container exits.
  name: exitCodes
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-container-restart-rule-schema.json
slug: argo-workflows-io-k8s-api-core-v1-container-restart-rule
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ContainerRestartRule
---

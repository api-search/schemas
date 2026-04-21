---
description: ContainerRestartRuleOnExitCodes describes the condition for handling an exited container based on its exit codes.
layout: schema
name: io.k8s.api.core.v1.ContainerRestartRuleOnExitCodes
properties_list:
- description: 'Represents the relationship between the container exit code(s) and the specified values. Possible values are: - In: the requirement is satisfied if the container exit code is in the set of specified v'
  name: operator
  type: string
- description: Specifies the set of values to check for container exit codes. At most 255 elements are allowed.
  name: values
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-container-restart-rule-on-exit-codes-schema.json
slug: argo-workflows-io-k8s-api-core-v1-container-restart-rule-on-exit-codes
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ContainerRestartRuleOnExitCodes
---

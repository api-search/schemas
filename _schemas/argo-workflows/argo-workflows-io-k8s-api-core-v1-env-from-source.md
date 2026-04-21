---
description: EnvFromSource represents the source of a set of ConfigMaps or Secrets
layout: schema
name: io.k8s.api.core.v1.EnvFromSource
properties_list:
- description: The ConfigMap to select from
  name: configMapRef
  type: object
- description: Optional text to prepend to the name of each environment variable. May consist of any printable ASCII characters except '='.
  name: prefix
  type: string
- description: The Secret to select from
  name: secretRef
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-env-from-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-env-from-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EnvFromSource
---

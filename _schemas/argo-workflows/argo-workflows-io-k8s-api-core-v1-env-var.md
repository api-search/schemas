---
description: EnvVar represents an environment variable present in a Container.
layout: schema
name: io.k8s.api.core.v1.EnvVar
properties_list:
- description: Name of the environment variable. May consist of any printable ASCII characters except '='.
  name: name
  type: string
- description: 'Variable references $(VAR_NAME) are expanded using the previously defined environment variables in the container and any service environment variables. If a variable cannot be resolved, the reference '
  name: value
  type: string
- description: Source for the environment variable's value. Cannot be used if value is not empty.
  name: valueFrom
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-env-var-schema.json
slug: argo-workflows-io-k8s-api-core-v1-env-var
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EnvVar
---

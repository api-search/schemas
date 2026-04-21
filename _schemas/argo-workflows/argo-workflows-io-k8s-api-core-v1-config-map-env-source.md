---
description: ConfigMapEnvSource selects a ConfigMap to populate the environment variables with. The contents of the target ConfigMap's Data field will represent the key-value pairs as environment variables.
layout: schema
name: io.k8s.api.core.v1.ConfigMapEnvSource
properties_list:
- description: Name of the referent. This field is effectively required, but due to backwards compatibility is allowed to be empty. Instances of this type with an empty value here are almost certainly wrong. More in
  name: name
  type: string
- description: Specify whether the ConfigMap must be defined
  name: optional
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-config-map-env-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-config-map-env-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ConfigMapEnvSource
---

---
description: SecretKeySelector selects a key of a Secret.
layout: schema
name: io.k8s.api.core.v1.SecretKeySelector
properties_list:
- description: The key of the secret to select from. Must be a valid secret key.
  name: key
  type: string
- description: Name of the referent. This field is effectively required, but due to backwards compatibility is allowed to be empty. Instances of this type with an empty value here are almost certainly wrong. More in
  name: name
  type: string
- description: Specify whether the Secret or its key must be defined
  name: optional
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-secret-key-selector-schema.json
slug: argo-workflows-io-k8s-api-core-v1-secret-key-selector
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.SecretKeySelector
---

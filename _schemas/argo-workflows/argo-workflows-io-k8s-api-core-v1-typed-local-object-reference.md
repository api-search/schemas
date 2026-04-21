---
description: TypedLocalObjectReference contains enough information to let you locate the typed referenced object inside the same namespace.
layout: schema
name: io.k8s.api.core.v1.TypedLocalObjectReference
properties_list:
- description: APIGroup is the group for the resource being referenced. If APIGroup is not specified, the specified Kind must be in the core API group. For any other third-party types, APIGroup is required.
  name: apiGroup
  type: string
- description: Kind is the type of resource being referenced
  name: kind
  type: string
- description: Name is the name of resource being referenced
  name: name
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-typed-local-object-reference-schema.json
slug: argo-workflows-io-k8s-api-core-v1-typed-local-object-reference
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.TypedLocalObjectReference
---

---
description: TypedObjectReference contains enough information to let you locate the typed referenced object
layout: schema
name: io.k8s.api.core.v1.TypedObjectReference
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
- description: Namespace is the namespace of resource being referenced Note that when a namespace is specified, a gateway.networking.k8s.io/ReferenceGrant object is required in the referent namespace to allow that n
  name: namespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-typed-object-reference-schema.json
slug: argo-workflows-io-k8s-api-core-v1-typed-object-reference
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.TypedObjectReference
---

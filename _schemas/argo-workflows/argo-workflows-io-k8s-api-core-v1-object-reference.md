---
description: ObjectReference contains enough information to let you inspect or modify the referred object.
layout: schema
name: io.k8s.api.core.v1.ObjectReference
properties_list:
- description: API version of the referent.
  name: apiVersion
  type: string
- description: If referring to a piece of an object instead of an entire object, this string should contain a valid JSON/Go field access statement, such as desiredState.manifest.containers[2]. For example, if the ob
  name: fieldPath
  type: string
- description: 'Kind of the referent. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds'
  name: kind
  type: string
- description: 'Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names'
  name: name
  type: string
- description: 'Namespace of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/'
  name: namespace
  type: string
- description: 'Specific resourceVersion to which this reference is made, if any. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency'
  name: resourceVersion
  type: string
- description: 'UID of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#uids'
  name: uid
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-object-reference-schema.json
slug: argo-workflows-io-k8s-api-core-v1-object-reference
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ObjectReference
---

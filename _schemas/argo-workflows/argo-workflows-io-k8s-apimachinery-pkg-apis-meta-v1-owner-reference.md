---
description: OwnerReference contains enough information to let you identify an owning object. An owning object must be in the same namespace as the dependent, or be cluster-scoped, so there is no namespace field.
layout: schema
name: io.k8s.apimachinery.pkg.apis.meta.v1.OwnerReference
properties_list:
- description: API version of the referent.
  name: apiVersion
  type: string
- description: If true, AND if the owner has the "foregroundDeletion" finalizer, then the owner cannot be deleted from the key-value store until this reference is removed. See https://kubernetes.io/docs/concepts/arc
  name: blockOwnerDeletion
  type: boolean
- description: If true, this reference points to the managing controller.
  name: controller
  type: boolean
- description: 'Kind of the referent. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds'
  name: kind
  type: string
- description: 'Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names'
  name: name
  type: string
- description: 'UID of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids'
  name: uid
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-owner-reference-schema.json
slug: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-owner-reference
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.apimachinery.pkg.apis.meta.v1.OwnerReference
---

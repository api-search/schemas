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
source_filename: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-owner-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-owner-reference-schema.json\",\n  \"title\": \"io.k8s.apimachinery.pkg.apis.meta.v1.OwnerReference\",\n  \"description\": \"OwnerReference contains enough information to let you identify an owning object. An owning object must be in the same namespace as the dependent, or be cluster-scoped, so there is no namespace field.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"description\": \"API version of the referent.\",\n      \"type\": \"string\"\n    },\n    \"blockOwnerDeletion\": {\n      \"description\": \"If true, AND if the owner has the \\\"foregroundDeletion\\\" finalizer, then the owner cannot be deleted from the key-value store until this reference is removed. See https://kubernetes.io/docs/concepts/architecture/garbage-collection/#foreground-deletion\
  \ for how the garbage collector interacts with this field and enforces the foreground deletion. Defaults to false. To set this field, a user needs \\\"delete\\\" permission of the owner, otherwise 422 (Unprocessable Entity) will be returned.\",\n      \"type\": \"boolean\"\n    },\n    \"controller\": {\n      \"description\": \"If true, this reference points to the managing controller.\",\n      \"type\": \"boolean\"\n    },\n    \"kind\": {\n      \"description\": \"Kind of the referent. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names\",\n      \"type\": \"string\"\n    },\n    \"uid\": {\n      \"description\": \"UID of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids\",\n      \"type\"\
  : \"string\"\n    }\n  },\n  \"required\": [\n    \"apiVersion\",\n    \"kind\",\n    \"name\",\n    \"uid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-owner-reference-schema.json
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

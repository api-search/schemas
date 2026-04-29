---
description: v1OwnerReference schema from Argo CD API
layout: schema
name: v1OwnerReference
properties_list:
- description: API version of the referent.
  name: apiVersion
  type: string
- description: ''
  name: blockOwnerDeletion
  type: boolean
- description: ''
  name: controller
  type: boolean
- description: ''
  name: kind
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: uid
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-owner-reference-schema.json
slug: argo-cd-v1-owner-reference
source_filename: argo-cd-v1-owner-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-owner-reference-schema.json\",\n  \"title\": \"v1OwnerReference\",\n  \"description\": \"v1OwnerReference schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"description\": \"API version of the referent.\",\n      \"type\": \"string\"\n    },\n    \"blockOwnerDeletion\": {\n      \"type\": \"boolean\",\n      \"title\": \"If true, AND if the owner has the \\\"foregroundDeletion\\\" finalizer, then\\nthe owner cannot be deleted from the key-value store until this\\nreference is removed.\\nSee https://kubernetes.io/docs/concepts/architecture/garbage-collection/#foreground-deletion\\nfor how the garbage collector interacts with this field and enforces the foreground deletion.\\nDefaults to false.\\nTo set this field, a user needs \\\"delete\\\" permission\
  \ of the owner,\\notherwise 422 (Unprocessable Entity) will be returned.\\n+optional\"\n    },\n    \"controller\": {\n      \"type\": \"boolean\",\n      \"title\": \"If true, this reference points to the managing controller.\\n+optional\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"title\": \"Kind of the referent.\\nMore info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name of the referent.\\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"title\": \"UID of the referent.\\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-owner-reference-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1OwnerReference
---

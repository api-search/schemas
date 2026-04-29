---
description: PersistentVolumeClaim is a user's request for and claim to a persistent volume
layout: schema
name: io.k8s.api.core.v1.PersistentVolumeClaim
properties_list:
- description: 'APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: http'
  name: apiVersion
  type: string
- description: 'Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https'
  name: kind
  type: string
- description: 'Standard object''s metadata. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata'
  name: metadata
  type: object
- description: 'spec defines the desired characteristics of a volume requested by a pod author. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims'
  name: spec
  type: object
- description: 'status represents the current information/status of a persistent volume claim. Read-only. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims'
  name: status
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-schema.json
slug: argo-workflows-io-k8s-api-core-v1-persistent-volume-claim
source_filename: argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PersistentVolumeClaim\",\n  \"description\": \"PersistentVolumeClaim is a user's request for and claim to a persistent volume\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"description\": \"APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources\",\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"description\": \"Kind is a string value representing the REST resource this object represents. Servers may infer this from the\
  \ endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"description\": \"Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.ObjectMeta\"\n    },\n    \"spec\": {\n      \"description\": \"spec defines the desired characteristics of a volume requested by a pod author. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PersistentVolumeClaimSpec\"\n    },\n    \"status\": {\n      \"description\": \"status represents the current information/status of a persistent volume claim. Read-only. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims\"\
  ,\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PersistentVolumeClaimStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PersistentVolumeClaim
---

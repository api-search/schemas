---
description: PersistentVolumeClaimVolumeSource references the user's PVC in the same namespace. This volume finds the bound PV and mounts that volume for the pod. A PersistentVolumeClaimVolumeSource is, essentially, a wrapper around another type of volume that is owned by someone else (the system).
layout: schema
name: io.k8s.api.core.v1.PersistentVolumeClaimVolumeSource
properties_list:
- description: 'claimName is the name of a PersistentVolumeClaim in the same namespace as the pod using this volume. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims'
  name: claimName
  type: string
- description: readOnly Will force the ReadOnly setting in VolumeMounts. Default false.
  name: readOnly
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PersistentVolumeClaimVolumeSource\",\n  \"description\": \"PersistentVolumeClaimVolumeSource references the user's PVC in the same namespace. This volume finds the bound PV and mounts that volume for the pod. A PersistentVolumeClaimVolumeSource is, essentially, a wrapper around another type of volume that is owned by someone else (the system).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"claimName\": {\n      \"description\": \"claimName is the name of a PersistentVolumeClaim in the same namespace as the pod using this volume. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims\",\n      \"type\": \"string\"\n    },\n    \"readOnly\"\
  : {\n      \"description\": \"readOnly Will force the ReadOnly setting in VolumeMounts. Default false.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"claimName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PersistentVolumeClaimVolumeSource
---

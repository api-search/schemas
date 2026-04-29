---
description: Represents a Ceph Filesystem mount that lasts the lifetime of a pod Cephfs volumes do not support ownership management or SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.CephFSVolumeSource
properties_list:
- description: 'monitors is Required: Monitors is a collection of Ceph monitors More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it'
  name: monitors
  type: array
- description: 'path is Optional: Used as the mounted root, rather than the full Ceph tree, default is /'
  name: path
  type: string
- description: 'readOnly is Optional: Defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts. More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it'
  name: readOnly
  type: boolean
- description: 'secretFile is Optional: SecretFile is the path to key ring for User, default is /etc/ceph/user.secret More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it'
  name: secretFile
  type: string
- description: 'secretRef is Optional: SecretRef is reference to the authentication secret for User, default is empty. More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it'
  name: secretRef
  type: object
- description: 'user is optional: User is the rados user name, default is admin More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it'
  name: user
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-ceph-fs-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-ceph-fs-volume-source
source_filename: argo-workflows-io-k8s-api-core-v1-ceph-fs-volume-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-ceph-fs-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.CephFSVolumeSource\",\n  \"description\": \"Represents a Ceph Filesystem mount that lasts the lifetime of a pod Cephfs volumes do not support ownership management or SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"monitors\": {\n      \"description\": \"monitors is Required: Monitors is a collection of Ceph monitors More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"path\": {\n      \"description\": \"path is Optional: Used as the mounted root, rather than the full Ceph tree, default is /\",\n      \"\
  type\": \"string\"\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly is Optional: Defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts. More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it\",\n      \"type\": \"boolean\"\n    },\n    \"secretFile\": {\n      \"description\": \"secretFile is Optional: SecretFile is the path to key ring for User, default is /etc/ceph/user.secret More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it\",\n      \"type\": \"string\"\n    },\n    \"secretRef\": {\n      \"description\": \"secretRef is Optional: SecretRef is reference to the authentication secret for User, default is empty. More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.LocalObjectReference\"\n    },\n    \"user\": {\n      \"description\": \"user is optional: User is the rados user name, default is admin More info: https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it\"\
  ,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"monitors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-ceph-fs-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.CephFSVolumeSource
---

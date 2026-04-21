---
description: Represents a Rados Block Device mount that lasts the lifetime of a pod. RBD volumes support ownership management and SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.RBDVolumeSource
properties_list:
- description: 'fsType is the filesystem type of the volume that you want to mount. Tip: Ensure that the filesystem type is supported by the host operating system. Examples: "ext4", "xfs", "ntfs". Implicitly inferred'
  name: fsType
  type: string
- description: 'image is the rados image name. More info: https://examples.k8s.io/volumes/rbd/README.md#how-to-use-it'
  name: image
  type: string
- description: 'keyring is the path to key ring for RBDUser. Default is /etc/ceph/keyring. More info: https://examples.k8s.io/volumes/rbd/README.md#how-to-use-it'
  name: keyring
  type: string
- description: 'monitors is a collection of Ceph monitors. More info: https://examples.k8s.io/volumes/rbd/README.md#how-to-use-it'
  name: monitors
  type: array
- description: 'pool is the rados pool name. Default is rbd. More info: https://examples.k8s.io/volumes/rbd/README.md#how-to-use-it'
  name: pool
  type: string
- description: 'readOnly here will force the ReadOnly setting in VolumeMounts. Defaults to false. More info: https://examples.k8s.io/volumes/rbd/README.md#how-to-use-it'
  name: readOnly
  type: boolean
- description: 'secretRef is name of the authentication secret for RBDUser. If provided overrides keyring. Default is nil. More info: https://examples.k8s.io/volumes/rbd/README.md#how-to-use-it'
  name: secretRef
  type: object
- description: 'user is the rados user name. Default is admin. More info: https://examples.k8s.io/volumes/rbd/README.md#how-to-use-it'
  name: user
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-rbd-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-rbd-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.RBDVolumeSource
---

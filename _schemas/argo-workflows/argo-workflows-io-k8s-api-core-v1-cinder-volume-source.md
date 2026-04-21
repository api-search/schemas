---
description: Represents a cinder volume resource in Openstack. A Cinder volume must exist before mounting to a container. The volume must also be in the same region as the kubelet. Cinder volumes support ownership management and SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.CinderVolumeSource
properties_list:
- description: 'fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Examples: "ext4", "xfs", "ntfs". Implicitly inferred to be "ext4" if unspecified. More info: h'
  name: fsType
  type: string
- description: 'readOnly defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts. More info: https://examples.k8s.io/mysql-cinder-pd/README.md'
  name: readOnly
  type: boolean
- description: 'secretRef is optional: points to a secret object containing parameters used to connect to OpenStack.'
  name: secretRef
  type: object
- description: 'volumeID used to identify the volume in cinder. More info: https://examples.k8s.io/mysql-cinder-pd/README.md'
  name: volumeID
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-cinder-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-cinder-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.CinderVolumeSource
---

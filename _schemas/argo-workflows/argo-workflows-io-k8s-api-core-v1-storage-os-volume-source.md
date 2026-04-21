---
description: Represents a StorageOS persistent volume resource.
layout: schema
name: io.k8s.api.core.v1.StorageOSVolumeSource
properties_list:
- description: fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to be "ext4" if unspecified.
  name: fsType
  type: string
- description: readOnly defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.
  name: readOnly
  type: boolean
- description: secretRef specifies the secret to use for obtaining the StorageOS API credentials. If not specified, default values will be attempted.
  name: secretRef
  type: object
- description: volumeName is the human-readable name of the StorageOS volume. Volume names are only unique within a namespace.
  name: volumeName
  type: string
- description: volumeNamespace specifies the scope of the volume within StorageOS. If no namespace is specified then the Pod's namespace will be used. This allows the Kubernetes name scoping to be mirrored within St
  name: volumeNamespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-storage-os-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-storage-os-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.StorageOSVolumeSource
---

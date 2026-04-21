---
description: Represents a Fibre Channel volume. Fibre Channel volumes can only be mounted as read/write once. Fibre Channel volumes support ownership management and SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.FCVolumeSource
properties_list:
- description: fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to be "ext4" if unspecified.
  name: fsType
  type: string
- description: 'lun is Optional: FC target lun number'
  name: lun
  type: integer
- description: 'readOnly is Optional: Defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.'
  name: readOnly
  type: boolean
- description: 'targetWWNs is Optional: FC target worldwide names (WWNs)'
  name: targetWWNs
  type: array
- description: 'wwids Optional: FC volume world wide identifiers (wwids) Either wwids or combination of targetWWNs and lun must be set, but not both simultaneously.'
  name: wwids
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-fc-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-fc-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.FCVolumeSource
---

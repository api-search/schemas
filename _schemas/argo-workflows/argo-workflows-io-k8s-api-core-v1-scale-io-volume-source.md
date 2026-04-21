---
description: ScaleIOVolumeSource represents a persistent ScaleIO volume
layout: schema
name: io.k8s.api.core.v1.ScaleIOVolumeSource
properties_list:
- description: fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. "ext4", "xfs", "ntfs". Default is "xfs".
  name: fsType
  type: string
- description: gateway is the host address of the ScaleIO API Gateway.
  name: gateway
  type: string
- description: protectionDomain is the name of the ScaleIO Protection Domain for the configured storage.
  name: protectionDomain
  type: string
- description: readOnly Defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.
  name: readOnly
  type: boolean
- description: secretRef references to the secret for ScaleIO user and other sensitive information. If this is not provided, Login operation will fail.
  name: secretRef
  type: object
- description: sslEnabled Flag enable/disable SSL communication with Gateway, default false
  name: sslEnabled
  type: boolean
- description: storageMode indicates whether the storage for a volume should be ThickProvisioned or ThinProvisioned. Default is ThinProvisioned.
  name: storageMode
  type: string
- description: storagePool is the ScaleIO Storage Pool associated with the protection domain.
  name: storagePool
  type: string
- description: system is the name of the storage system as configured in ScaleIO.
  name: system
  type: string
- description: volumeName is the name of a volume already created in the ScaleIO system that is associated with this volume source.
  name: volumeName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-scale-io-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-scale-io-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ScaleIOVolumeSource
---

---
description: AzureDisk represents an Azure Data Disk mount on the host and bind mount to the pod.
layout: schema
name: io.k8s.api.core.v1.AzureDiskVolumeSource
properties_list:
- description: 'cachingMode is the Host Caching mode: None, Read Only, Read Write.'
  name: cachingMode
  type: string
- description: diskName is the Name of the data disk in the blob storage
  name: diskName
  type: string
- description: diskURI is the URI of data disk in the blob storage
  name: diskURI
  type: string
- description: fsType is Filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to be "ext4" if unspecified.
  name: fsType
  type: string
- description: 'kind expected values are Shared: multiple blob disks per storage account Dedicated: single blob disk per storage account Managed: azure managed data disk (only in managed availability set). defaults t'
  name: kind
  type: string
- description: readOnly Defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.
  name: readOnly
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-azure-disk-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-azure-disk-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.AzureDiskVolumeSource
---

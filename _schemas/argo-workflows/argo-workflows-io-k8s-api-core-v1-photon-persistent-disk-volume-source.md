---
description: Represents a Photon Controller persistent disk resource.
layout: schema
name: io.k8s.api.core.v1.PhotonPersistentDiskVolumeSource
properties_list:
- description: fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to be "ext4" if unspecified.
  name: fsType
  type: string
- description: pdID is the ID that identifies Photon Controller persistent disk
  name: pdID
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-photon-persistent-disk-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-photon-persistent-disk-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PhotonPersistentDiskVolumeSource
---

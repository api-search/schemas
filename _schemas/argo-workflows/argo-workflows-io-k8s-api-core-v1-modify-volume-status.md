---
description: ModifyVolumeStatus represents the status object of ControllerModifyVolume operation
layout: schema
name: io.k8s.api.core.v1.ModifyVolumeStatus
properties_list:
- description: 'status is the status of the ControllerModifyVolume operation. It can be in any of following states: - Pending Pending indicates that the PersistentVolumeClaim cannot be modified due to unmet requireme'
  name: status
  type: string
- description: targetVolumeAttributesClassName is the name of the VolumeAttributesClass the PVC currently being reconciled
  name: targetVolumeAttributesClassName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-modify-volume-status-schema.json
slug: argo-workflows-io-k8s-api-core-v1-modify-volume-status
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ModifyVolumeStatus
---

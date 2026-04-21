---
description: PersistentVolumeClaimStatus is the current status of a persistent volume claim.
layout: schema
name: io.k8s.api.core.v1.PersistentVolumeClaimStatus
properties_list:
- description: 'accessModes contains the actual access modes the volume backing the PVC has. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#access-modes-1'
  name: accessModes
  type: array
- description: 'allocatedResourceStatuses stores status of resource being resized for the given PVC. Key names follow standard Kubernetes label syntax. Valid values are either: * Un-prefixed keys: - storage - the cap'
  name: allocatedResourceStatuses
  type: object
- description: 'allocatedResources tracks the resources allocated to a PVC including its capacity. Key names follow standard Kubernetes label syntax. Valid values are either: * Un-prefixed keys: - storage - the capac'
  name: allocatedResources
  type: object
- description: capacity represents the actual resources of the underlying volume.
  name: capacity
  type: object
- description: conditions is the current Condition of persistent volume claim. If underlying persistent volume is being resized then the Condition will be set to 'Resizing'.
  name: conditions
  type: array
- description: currentVolumeAttributesClassName is the current name of the VolumeAttributesClass the PVC is using. When unset, there is no VolumeAttributeClass applied to this PersistentVolumeClaim
  name: currentVolumeAttributesClassName
  type: string
- description: ModifyVolumeStatus represents the status object of ControllerModifyVolume operation. When this is unset, there is no ModifyVolume operation being attempted.
  name: modifyVolumeStatus
  type: object
- description: phase represents the current phase of PersistentVolumeClaim.
  name: phase
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-status-schema.json
slug: argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-status
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PersistentVolumeClaimStatus
---

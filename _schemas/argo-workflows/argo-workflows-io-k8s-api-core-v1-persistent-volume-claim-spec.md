---
description: PersistentVolumeClaimSpec describes the common attributes of storage devices and allows a Source for provider-specific attributes
layout: schema
name: io.k8s.api.core.v1.PersistentVolumeClaimSpec
properties_list:
- description: 'accessModes contains the desired access modes the volume should have. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#access-modes-1'
  name: accessModes
  type: array
- description: 'dataSource field can be used to specify either: * An existing VolumeSnapshot object (snapshot.storage.k8s.io/VolumeSnapshot) * An existing PVC (PersistentVolumeClaim) If the provisioner or an external'
  name: dataSource
  type: object
- description: dataSourceRef specifies the object from which to populate the volume with data, if a non-empty volume is desired. This may be any object from a non-empty API group (non core object) or a PersistentVol
  name: dataSourceRef
  type: object
- description: resources represents the minimum resources the volume should have. Users are allowed to specify resource requirements that are lower than previous value but must still be higher than capacity recorded
  name: resources
  type: object
- description: selector is a label query over volumes to consider for binding.
  name: selector
  type: object
- description: 'storageClassName is the name of the StorageClass required by the claim. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#class-1'
  name: storageClassName
  type: string
- description: volumeAttributesClassName may be used to set the VolumeAttributesClass used by this claim. If specified, the CSI driver will create or update the volume with the attributes defined in the correspondin
  name: volumeAttributesClassName
  type: string
- description: volumeMode defines what type of volume is required by the claim. Value of Filesystem is implied when not included in claim spec.
  name: volumeMode
  type: string
- description: volumeName is the binding reference to the PersistentVolume backing this claim.
  name: volumeName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-spec-schema.json
slug: argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-spec
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PersistentVolumeClaimSpec
---

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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-status-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PersistentVolumeClaimStatus\",\n  \"description\": \"PersistentVolumeClaimStatus is the current status of a persistent volume claim.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessModes\": {\n      \"description\": \"accessModes contains the actual access modes the volume backing the PVC has. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#access-modes-1\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"allocatedResourceStatuses\": {\n      \"description\": \"allocatedResourceStatuses stores status of resource being resized for the given PVC. Key names\
  \ follow standard Kubernetes label syntax. Valid values are either:\\n\\t* Un-prefixed keys:\\n\\t\\t- storage - the capacity of the volume.\\n\\t* Custom resources must use implementation-defined prefixed names such as \\\"example.com/my-custom-resource\\\"\\nApart from above values - keys that are unprefixed or have kubernetes.io prefix are considered reserved and hence may not be used.\\n\\nClaimResourceStatus can be in any of following states:\\n\\t- ControllerResizeInProgress:\\n\\t\\tState set when resize controller starts resizing the volume in control-plane.\\n\\t- ControllerResizeFailed:\\n\\t\\tState set when resize has failed in resize controller with a terminal error.\\n\\t- NodeResizePending:\\n\\t\\tState set when resize controller has finished resizing the volume but further resizing of\\n\\t\\tvolume is needed on the node.\\n\\t- NodeResizeInProgress:\\n\\t\\tState set when kubelet starts resizing the volume.\\n\\t- NodeResizeFailed:\\n\\t\\tState set when resizing has\
  \ failed in kubelet with a terminal error. Transient errors don't set\\n\\t\\tNodeResizeFailed.\\nFor example: if expanding a PVC for more capacity - this field can be one of the following states:\\n\\t- pvc.status.allocatedResourceStatus['storage'] = \\\"ControllerResizeInProgress\\\"\\n     - pvc.status.allocatedResourceStatus['storage'] = \\\"ControllerResizeFailed\\\"\\n     - pvc.status.allocatedResourceStatus['storage'] = \\\"NodeResizePending\\\"\\n     - pvc.status.allocatedResourceStatus['storage'] = \\\"NodeResizeInProgress\\\"\\n     - pvc.status.allocatedResourceStatus['storage'] = \\\"NodeResizeFailed\\\"\\nWhen this field is not set, it means that no resize operation is in progress for the given PVC.\\n\\nA controller that receives PVC update with previously unknown resourceName or ClaimResourceStatus should ignore the update for the purpose it was designed. For example - a controller that only is responsible for resizing capacity of the volume, should ignore PVC updates\
  \ that change other valid resources associated with PVC.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-map-type\": \"granular\"\n    },\n    \"allocatedResources\": {\n      \"description\": \"allocatedResources tracks the resources allocated to a PVC including its capacity. Key names follow standard Kubernetes label syntax. Valid values are either:\\n\\t* Un-prefixed keys:\\n\\t\\t- storage - the capacity of the volume.\\n\\t* Custom resources must use implementation-defined prefixed names such as \\\"example.com/my-custom-resource\\\"\\nApart from above values - keys that are unprefixed or have kubernetes.io prefix are considered reserved and hence may not be used.\\n\\nCapacity reported here may be larger than the actual capacity when a volume expansion operation is requested. For storage quota, the larger value from allocatedResources and PVC.spec.resources is used. If allocatedResources is not set,\
  \ PVC.spec.resources alone is used for quota calculation. If a volume expansion capacity request is lowered, allocatedResources is only lowered if there are no expansion operations in progress and if the actual volume capacity is equal or lower than the requested capacity.\\n\\nA controller that receives PVC update with previously unknown resourceName should ignore the update for the purpose it was designed. For example - a controller that only is responsible for resizing capacity of the volume, should ignore PVC updates that change other valid resources associated with PVC.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.api.resource.Quantity\"\n      }\n    },\n    \"capacity\": {\n      \"description\": \"capacity represents the actual resources of the underlying volume.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.api.resource.Quantity\"\
  \n      }\n    },\n    \"conditions\": {\n      \"description\": \"conditions is the current Condition of persistent volume claim. If underlying persistent volume is being resized then the Condition will be set to 'Resizing'.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.PersistentVolumeClaimCondition\"\n      },\n      \"x-kubernetes-list-map-keys\": [\n        \"type\"\n      ],\n      \"x-kubernetes-list-type\": \"map\",\n      \"x-kubernetes-patch-merge-key\": \"type\",\n      \"x-kubernetes-patch-strategy\": \"merge\"\n    },\n    \"currentVolumeAttributesClassName\": {\n      \"description\": \"currentVolumeAttributesClassName is the current name of the VolumeAttributesClass the PVC is using. When unset, there is no VolumeAttributeClass applied to this PersistentVolumeClaim\",\n      \"type\": \"string\"\n    },\n    \"modifyVolumeStatus\": {\n      \"description\": \"ModifyVolumeStatus represents the status object of ControllerModifyVolume\
  \ operation. When this is unset, there is no ModifyVolume operation being attempted.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ModifyVolumeStatus\"\n    },\n    \"phase\": {\n      \"description\": \"phase represents the current phase of PersistentVolumeClaim.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-status-schema.json
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

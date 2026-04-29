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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-modify-volume-status-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ModifyVolumeStatus\",\n  \"description\": \"ModifyVolumeStatus represents the status object of ControllerModifyVolume operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"description\": \"status is the status of the ControllerModifyVolume operation. It can be in any of following states:\\n - Pending\\n   Pending indicates that the PersistentVolumeClaim cannot be modified due to unmet requirements, such as\\n   the specified VolumeAttributesClass not existing.\\n - InProgress\\n   InProgress indicates that the volume is being modified.\\n - Infeasible\\n  Infeasible indicates that the request has been rejected as invalid by the CSI driver. To\\n\\t  resolve the error,\
  \ a valid VolumeAttributesClass needs to be specified.\\nNote: New statuses can be added in the future. Consumers should check for unknown statuses and fail appropriately.\",\n      \"type\": \"string\"\n    },\n    \"targetVolumeAttributesClassName\": {\n      \"description\": \"targetVolumeAttributesClassName is the name of the VolumeAttributesClass the PVC currently being reconciled\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-modify-volume-status-schema.json
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

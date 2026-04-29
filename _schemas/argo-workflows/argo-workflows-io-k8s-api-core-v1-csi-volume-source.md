---
description: Represents a source location of a volume to mount, managed by an external CSI driver
layout: schema
name: io.k8s.api.core.v1.CSIVolumeSource
properties_list:
- description: driver is the name of the CSI driver that handles this volume. Consult with your admin for the correct name as registered in the cluster.
  name: driver
  type: string
- description: fsType to mount. Ex. "ext4", "xfs", "ntfs". If not provided, the empty value is passed to the associated CSI driver which will determine the default filesystem to apply.
  name: fsType
  type: string
- description: nodePublishSecretRef is a reference to the secret object containing sensitive information to pass to the CSI driver to complete the CSI NodePublishVolume and NodeUnpublishVolume calls. This field is o
  name: nodePublishSecretRef
  type: object
- description: readOnly specifies a read-only configuration for the volume. Defaults to false (read/write).
  name: readOnly
  type: boolean
- description: volumeAttributes stores driver-specific properties that are passed to the CSI driver. Consult your driver's documentation for supported values.
  name: volumeAttributes
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-csi-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-csi-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-csi-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.CSIVolumeSource\",\n  \"description\": \"Represents a source location of a volume to mount, managed by an external CSI driver\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"driver\": {\n      \"description\": \"driver is the name of the CSI driver that handles this volume. Consult with your admin for the correct name as registered in the cluster.\",\n      \"type\": \"string\"\n    },\n    \"fsType\": {\n      \"description\": \"fsType to mount. Ex. \\\"ext4\\\", \\\"xfs\\\", \\\"ntfs\\\". If not provided, the empty value is passed to the associated CSI driver which will determine the default filesystem to apply.\",\n      \"type\": \"string\"\n    },\n    \"nodePublishSecretRef\": {\n      \"\
  description\": \"nodePublishSecretRef is a reference to the secret object containing sensitive information to pass to the CSI driver to complete the CSI NodePublishVolume and NodeUnpublishVolume calls. This field is optional, and  may be empty if no secret is required. If the secret object contains more than one secret, all secret references are passed.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.LocalObjectReference\"\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly specifies a read-only configuration for the volume. Defaults to false (read/write).\",\n      \"type\": \"boolean\"\n    },\n    \"volumeAttributes\": {\n      \"description\": \"volumeAttributes stores driver-specific properties that are passed to the CSI driver. Consult your driver's documentation for supported values.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"driver\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-csi-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.CSIVolumeSource
---

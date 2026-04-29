---
description: Represents a vSphere volume resource.
layout: schema
name: io.k8s.api.core.v1.VsphereVirtualDiskVolumeSource
properties_list:
- description: fsType is filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to be "ext4" if unspecified.
  name: fsType
  type: string
- description: storagePolicyID is the storage Policy Based Management (SPBM) profile ID associated with the StoragePolicyName.
  name: storagePolicyID
  type: string
- description: storagePolicyName is the storage Policy Based Management (SPBM) profile name.
  name: storagePolicyName
  type: string
- description: volumePath is the path that identifies vSphere volume vmdk
  name: volumePath
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-vsphere-virtual-disk-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-vsphere-virtual-disk-volume-source
source_filename: argo-workflows-io-k8s-api-core-v1-vsphere-virtual-disk-volume-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-vsphere-virtual-disk-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.VsphereVirtualDiskVolumeSource\",\n  \"description\": \"Represents a vSphere volume resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsType\": {\n      \"description\": \"fsType is filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. \\\"ext4\\\", \\\"xfs\\\", \\\"ntfs\\\". Implicitly inferred to be \\\"ext4\\\" if unspecified.\",\n      \"type\": \"string\"\n    },\n    \"storagePolicyID\": {\n      \"description\": \"storagePolicyID is the storage Policy Based Management (SPBM) profile ID associated with the StoragePolicyName.\",\n      \"type\": \"string\"\n    },\n    \"storagePolicyName\": {\n      \"description\": \"storagePolicyName\
  \ is the storage Policy Based Management (SPBM) profile name.\",\n      \"type\": \"string\"\n    },\n    \"volumePath\": {\n      \"description\": \"volumePath is the path that identifies vSphere volume vmdk\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"volumePath\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-vsphere-virtual-disk-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.VsphereVirtualDiskVolumeSource
---

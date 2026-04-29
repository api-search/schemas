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
source_filename: argo-workflows-io-k8s-api-core-v1-photon-persistent-disk-volume-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-photon-persistent-disk-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PhotonPersistentDiskVolumeSource\",\n  \"description\": \"Represents a Photon Controller persistent disk resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsType\": {\n      \"description\": \"fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. \\\"ext4\\\", \\\"xfs\\\", \\\"ntfs\\\". Implicitly inferred to be \\\"ext4\\\" if unspecified.\",\n      \"type\": \"string\"\n    },\n    \"pdID\": {\n      \"description\": \"pdID is the ID that identifies Photon Controller persistent disk\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pdID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-photon-persistent-disk-volume-source-schema.json
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

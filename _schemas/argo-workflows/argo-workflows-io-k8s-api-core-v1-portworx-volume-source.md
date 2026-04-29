---
description: PortworxVolumeSource represents a Portworx volume resource.
layout: schema
name: io.k8s.api.core.v1.PortworxVolumeSource
properties_list:
- description: fSType represents the filesystem type to mount Must be a filesystem type supported by the host operating system. Ex. "ext4", "xfs". Implicitly inferred to be "ext4" if unspecified.
  name: fsType
  type: string
- description: readOnly defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.
  name: readOnly
  type: boolean
- description: volumeID uniquely identifies a Portworx volume
  name: volumeID
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-portworx-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-portworx-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-portworx-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PortworxVolumeSource\",\n  \"description\": \"PortworxVolumeSource represents a Portworx volume resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsType\": {\n      \"description\": \"fSType represents the filesystem type to mount Must be a filesystem type supported by the host operating system. Ex. \\\"ext4\\\", \\\"xfs\\\". Implicitly inferred to be \\\"ext4\\\" if unspecified.\",\n      \"type\": \"string\"\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.\",\n      \"type\": \"boolean\"\n    },\n    \"volumeID\": {\n      \"description\": \"volumeID uniquely identifies a\
  \ Portworx volume\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"volumeID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-portworx-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PortworxVolumeSource
---

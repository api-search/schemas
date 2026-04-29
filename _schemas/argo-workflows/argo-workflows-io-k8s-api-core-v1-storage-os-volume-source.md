---
description: Represents a StorageOS persistent volume resource.
layout: schema
name: io.k8s.api.core.v1.StorageOSVolumeSource
properties_list:
- description: fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to be "ext4" if unspecified.
  name: fsType
  type: string
- description: readOnly defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.
  name: readOnly
  type: boolean
- description: secretRef specifies the secret to use for obtaining the StorageOS API credentials. If not specified, default values will be attempted.
  name: secretRef
  type: object
- description: volumeName is the human-readable name of the StorageOS volume. Volume names are only unique within a namespace.
  name: volumeName
  type: string
- description: volumeNamespace specifies the scope of the volume within StorageOS. If no namespace is specified then the Pod's namespace will be used. This allows the Kubernetes name scoping to be mirrored within St
  name: volumeNamespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-storage-os-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-storage-os-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-storage-os-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.StorageOSVolumeSource\",\n  \"description\": \"Represents a StorageOS persistent volume resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsType\": {\n      \"description\": \"fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. \\\"ext4\\\", \\\"xfs\\\", \\\"ntfs\\\". Implicitly inferred to be \\\"ext4\\\" if unspecified.\",\n      \"type\": \"string\"\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.\",\n      \"type\": \"boolean\"\n    },\n    \"secretRef\": {\n      \"description\": \"secretRef specifies the secret\
  \ to use for obtaining the StorageOS API credentials.  If not specified, default values will be attempted.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.LocalObjectReference\"\n    },\n    \"volumeName\": {\n      \"description\": \"volumeName is the human-readable name of the StorageOS volume.  Volume names are only unique within a namespace.\",\n      \"type\": \"string\"\n    },\n    \"volumeNamespace\": {\n      \"description\": \"volumeNamespace specifies the scope of the volume within StorageOS.  If no namespace is specified then the Pod's namespace will be used.  This allows the Kubernetes name scoping to be mirrored within StorageOS for tighter integration. Set VolumeName to any name to override the default behaviour. Set to \\\"default\\\" if you are not using namespaces within StorageOS. Namespaces that do not pre-exist within StorageOS will be created.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-storage-os-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.StorageOSVolumeSource
---

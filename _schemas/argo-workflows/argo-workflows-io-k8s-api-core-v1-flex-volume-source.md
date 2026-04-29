---
description: FlexVolume represents a generic volume resource that is provisioned/attached using an exec based plugin.
layout: schema
name: io.k8s.api.core.v1.FlexVolumeSource
properties_list:
- description: driver is the name of the driver to use for this volume.
  name: driver
  type: string
- description: fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. "ext4", "xfs", "ntfs". The default filesystem depends on FlexVolume script.
  name: fsType
  type: string
- description: 'options is Optional: this field holds extra command options if any.'
  name: options
  type: object
- description: 'readOnly is Optional: defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.'
  name: readOnly
  type: boolean
- description: 'secretRef is Optional: secretRef is reference to the secret object containing sensitive information to pass to the plugin scripts. This may be empty if no secret object is specified. If the secret obj'
  name: secretRef
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-flex-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-flex-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-flex-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.FlexVolumeSource\",\n  \"description\": \"FlexVolume represents a generic volume resource that is provisioned/attached using an exec based plugin.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"driver\": {\n      \"description\": \"driver is the name of the driver to use for this volume.\",\n      \"type\": \"string\"\n    },\n    \"fsType\": {\n      \"description\": \"fsType is the filesystem type to mount. Must be a filesystem type supported by the host operating system. Ex. \\\"ext4\\\", \\\"xfs\\\", \\\"ntfs\\\". The default filesystem depends on FlexVolume script.\",\n      \"type\": \"string\"\n    },\n    \"options\": {\n      \"description\": \"options is Optional: this field holds extra\
  \ command options if any.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly is Optional: defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.\",\n      \"type\": \"boolean\"\n    },\n    \"secretRef\": {\n      \"description\": \"secretRef is Optional: secretRef is reference to the secret object containing sensitive information to pass to the plugin scripts. This may be empty if no secret object is specified. If the secret object contains more than one secret, all secrets are passed to the plugin scripts.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.LocalObjectReference\"\n    }\n  },\n  \"required\": [\n    \"driver\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-flex-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.FlexVolumeSource
---

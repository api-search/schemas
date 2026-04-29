---
description: VolumeMount describes a mounting of a Volume within a container.
layout: schema
name: io.k8s.api.core.v1.VolumeMount
properties_list:
- description: Path within the container at which the volume should be mounted. Must not contain ':'.
  name: mountPath
  type: string
- description: mountPropagation determines how mounts are propagated from the host to container and the other way around. When not set, MountPropagationNone is used. This field is beta in 1.10. When RecursiveReadOnl
  name: mountPropagation
  type: string
- description: This must match the Name of a Volume.
  name: name
  type: string
- description: Mounted read-only if true, read-write otherwise (false or unspecified). Defaults to false.
  name: readOnly
  type: boolean
- description: 'RecursiveReadOnly specifies whether read-only mounts should be handled recursively. If ReadOnly is false, this field has no meaning and must be unspecified. If ReadOnly is true, and this field is set '
  name: recursiveReadOnly
  type: string
- description: Path within the volume from which the container's volume should be mounted. Defaults to "" (volume's root).
  name: subPath
  type: string
- description: Expanded path within the volume from which the container's volume should be mounted. Behaves similarly to SubPath but environment variable references $(VAR_NAME) are expanded using the container's env
  name: subPathExpr
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-volume-mount-schema.json
slug: argo-workflows-io-k8s-api-core-v1-volume-mount
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-volume-mount-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.VolumeMount\",\n  \"description\": \"VolumeMount describes a mounting of a Volume within a container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mountPath\": {\n      \"description\": \"Path within the container at which the volume should be mounted.  Must not contain ':'.\",\n      \"type\": \"string\"\n    },\n    \"mountPropagation\": {\n      \"description\": \"mountPropagation determines how mounts are propagated from the host to container and the other way around. When not set, MountPropagationNone is used. This field is beta in 1.10. When RecursiveReadOnly is set to IfPossible or to Enabled, MountPropagation must be None or unspecified (which defaults to None).\",\n      \"type\": \"string\"\
  \n    },\n    \"name\": {\n      \"description\": \"This must match the Name of a Volume.\",\n      \"type\": \"string\"\n    },\n    \"readOnly\": {\n      \"description\": \"Mounted read-only if true, read-write otherwise (false or unspecified). Defaults to false.\",\n      \"type\": \"boolean\"\n    },\n    \"recursiveReadOnly\": {\n      \"description\": \"RecursiveReadOnly specifies whether read-only mounts should be handled recursively.\\n\\nIf ReadOnly is false, this field has no meaning and must be unspecified.\\n\\nIf ReadOnly is true, and this field is set to Disabled, the mount is not made recursively read-only.  If this field is set to IfPossible, the mount is made recursively read-only, if it is supported by the container runtime.  If this field is set to Enabled, the mount is made recursively read-only if it is supported by the container runtime, otherwise the pod will not be started and an error will be generated to indicate the reason.\\n\\nIf this field is set to IfPossible\
  \ or Enabled, MountPropagation must be set to None (or be unspecified, which defaults to None).\\n\\nIf this field is not specified, it is treated as an equivalent of Disabled.\",\n      \"type\": \"string\"\n    },\n    \"subPath\": {\n      \"description\": \"Path within the volume from which the container's volume should be mounted. Defaults to \\\"\\\" (volume's root).\",\n      \"type\": \"string\"\n    },\n    \"subPathExpr\": {\n      \"description\": \"Expanded path within the volume from which the container's volume should be mounted. Behaves similarly to SubPath but environment variable references $(VAR_NAME) are expanded using the container's environment. Defaults to \\\"\\\" (volume's root). SubPathExpr and SubPath are mutually exclusive.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"mountPath\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-volume-mount-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.VolumeMount
---

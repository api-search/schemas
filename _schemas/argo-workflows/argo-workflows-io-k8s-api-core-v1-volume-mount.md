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

---
description: volumeDevice describes a mapping of a raw block device within a container.
layout: schema
name: io.k8s.api.core.v1.VolumeDevice
properties_list:
- description: devicePath is the path inside of the container that the device will be mapped to.
  name: devicePath
  type: string
- description: name must match the name of a persistentVolumeClaim in the pod
  name: name
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-volume-device-schema.json
slug: argo-workflows-io-k8s-api-core-v1-volume-device
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.VolumeDevice
---

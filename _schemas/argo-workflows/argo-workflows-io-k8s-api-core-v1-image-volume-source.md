---
description: ImageVolumeSource represents a image volume resource.
layout: schema
name: io.k8s.api.core.v1.ImageVolumeSource
properties_list:
- description: 'Policy for pulling OCI objects. Possible values are: Always: the kubelet always attempts to pull the reference. Container creation will fail If the pull fails. Never: the kubelet never pulls the refer'
  name: pullPolicy
  type: string
- description: 'Required: Image or artifact reference to be used. Behaves in the same way as pod.spec.containers[*].image. Pull secrets will be assembled in the same way as for the container image by looking up node '
  name: reference
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-image-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-image-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ImageVolumeSource
---

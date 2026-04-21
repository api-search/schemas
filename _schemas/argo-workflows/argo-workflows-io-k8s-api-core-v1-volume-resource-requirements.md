---
description: VolumeResourceRequirements describes the storage resource requirements for a volume.
layout: schema
name: io.k8s.api.core.v1.VolumeResourceRequirements
properties_list:
- description: 'Limits describes the maximum amount of compute resources allowed. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/'
  name: limits
  type: object
- description: Requests describes the minimum amount of compute resources required. If Requests is omitted for a container, it defaults to Limits if that is explicitly specified, otherwise to an implementation-defin
  name: requests
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-volume-resource-requirements-schema.json
slug: argo-workflows-io-k8s-api-core-v1-volume-resource-requirements
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.VolumeResourceRequirements
---

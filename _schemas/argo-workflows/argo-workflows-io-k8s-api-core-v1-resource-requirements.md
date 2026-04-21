---
description: ResourceRequirements describes the compute resource requirements.
layout: schema
name: io.k8s.api.core.v1.ResourceRequirements
properties_list:
- description: 'Claims lists the names of resources, defined in spec.resourceClaims, that are used by this container. This field depends on the DynamicResourceAllocation feature gate. This field is immutable. It can '
  name: claims
  type: array
- description: 'Limits describes the maximum amount of compute resources allowed. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/'
  name: limits
  type: object
- description: Requests describes the minimum amount of compute resources required. If Requests is omitted for a container, it defaults to Limits if that is explicitly specified, otherwise to an implementation-defin
  name: requests
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-resource-requirements-schema.json
slug: argo-workflows-io-k8s-api-core-v1-resource-requirements
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ResourceRequirements
---

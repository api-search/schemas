---
description: SeccompProfile defines a pod/container's seccomp profile settings. Only one profile source may be set.
layout: schema
name: io.k8s.api.core.v1.SeccompProfile
properties_list:
- description: localhostProfile indicates a profile defined in a file on the node should be used. The profile must be preconfigured on the node to work. Must be a descending path, relative to the kubelet's configure
  name: localhostProfile
  type: string
- description: 'type indicates which kind of seccomp profile will be applied. Valid options are: Localhost - a profile defined in a file on the node should be used. RuntimeDefault - the container runtime default prof'
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-seccomp-profile-schema.json
slug: argo-workflows-io-k8s-api-core-v1-seccomp-profile
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.SeccompProfile
---

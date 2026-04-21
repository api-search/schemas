---
description: HostAlias holds the mapping between IP and hostnames that will be injected as an entry in the pod's hosts file.
layout: schema
name: io.k8s.api.core.v1.HostAlias
properties_list:
- description: Hostnames for the above IP address.
  name: hostnames
  type: array
- description: IP address of the host file entry.
  name: ip
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-host-alias-schema.json
slug: argo-workflows-io-k8s-api-core-v1-host-alias
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.HostAlias
---

---
description: ContainerPort represents a network port in a single container.
layout: schema
name: io.k8s.api.core.v1.ContainerPort
properties_list:
- description: Number of port to expose on the pod's IP address. This must be a valid port number, 0 < x < 65536.
  name: containerPort
  type: integer
- description: What host IP to bind the external port to.
  name: hostIP
  type: string
- description: Number of port to expose on the host. If specified, this must be a valid port number, 0 < x < 65536. If HostNetwork is specified, this must match ContainerPort. Most containers do not need this.
  name: hostPort
  type: integer
- description: If specified, this must be an IANA_SVC_NAME and unique within the pod. Each named port in a pod must have a unique name. Name for the port that can be referred to by services.
  name: name
  type: string
- description: Protocol for port. Must be UDP, TCP, or SCTP. Defaults to "TCP".
  name: protocol
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-container-port-schema.json
slug: argo-workflows-io-k8s-api-core-v1-container-port
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ContainerPort
---

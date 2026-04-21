---
description: TCPSocketAction describes an action based on opening a socket
layout: schema
name: io.k8s.api.core.v1.TCPSocketAction
properties_list:
- description: 'Optional: Host name to connect to, defaults to the pod IP.'
  name: host
  type: string
- description: Number or name of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME.
  name: port
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-tcp-socket-action-schema.json
slug: argo-workflows-io-k8s-api-core-v1-tcp-socket-action
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.TCPSocketAction
---

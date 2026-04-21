---
description: LifecycleHandler defines a specific action that should be taken in a lifecycle hook. One and only one of the fields, except TCPSocket must be specified.
layout: schema
name: io.k8s.api.core.v1.LifecycleHandler
properties_list:
- description: Exec specifies a command to execute in the container.
  name: exec
  type: object
- description: HTTPGet specifies an HTTP GET request to perform.
  name: httpGet
  type: object
- description: Sleep represents a duration that the container should sleep.
  name: sleep
  type: object
- description: Deprecated. TCPSocket is NOT supported as a LifecycleHandler and kept for backward compatibility. There is no validation of this field and lifecycle hooks will fail at runtime when it is specified.
  name: tcpSocket
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-lifecycle-handler-schema.json
slug: argo-workflows-io-k8s-api-core-v1-lifecycle-handler
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.LifecycleHandler
---

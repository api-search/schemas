---
description: HTTPGetAction describes an action based on HTTP Get requests.
layout: schema
name: io.k8s.api.core.v1.HTTPGetAction
properties_list:
- description: Host name to connect to, defaults to the pod IP. You probably want to set "Host" in httpHeaders instead.
  name: host
  type: string
- description: Custom headers to set in the request. HTTP allows repeated headers.
  name: httpHeaders
  type: array
- description: Path to access on the HTTP server.
  name: path
  type: string
- description: Name or number of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME.
  name: port
  type: object
- description: Scheme to use for connecting to the host. Defaults to HTTP.
  name: scheme
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-http-get-action-schema.json
slug: argo-workflows-io-k8s-api-core-v1-http-get-action
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.HTTPGetAction
---

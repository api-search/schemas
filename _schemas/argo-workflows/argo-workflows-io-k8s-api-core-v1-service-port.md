---
description: ServicePort contains information on service's port.
layout: schema
name: io.k8s.api.core.v1.ServicePort
properties_list:
- description: The application protocol for this port. This is used as a hint for implementations to offer richer behavior for protocols that they understand. This field follows standard Kubernetes label syntax. Val
  name: appProtocol
  type: string
- description: The name of this port within the service. This must be a DNS_LABEL. All ports within a ServiceSpec must have unique names. When considering the endpoints for a Service, this must match the 'name' fiel
  name: name
  type: string
- description: The port on each node on which this service is exposed when type is NodePort or LoadBalancer. Usually assigned by the system. If a value is specified, in-range, and not in use it will be used, otherwi
  name: nodePort
  type: integer
- description: The port that will be exposed by this service.
  name: port
  type: integer
- description: The IP protocol for this port. Supports "TCP", "UDP", and "SCTP". Default is TCP.
  name: protocol
  type: string
- description: Number or name of the port to access on the pods targeted by the service. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME. If this is a string, it will be looked up as a named po
  name: targetPort
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-service-port-schema.json
slug: argo-workflows-io-k8s-api-core-v1-service-port
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ServicePort
---

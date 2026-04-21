---
description: GRPCAction specifies an action involving a GRPC service.
layout: schema
name: io.k8s.api.core.v1.GRPCAction
properties_list:
- description: Port number of the gRPC service. Number must be in the range 1 to 65535.
  name: port
  type: integer
- description: Service is the name of the service to place in the gRPC HealthCheckRequest (see https://github.com/grpc/grpc/blob/master/doc/health-checking.md). If this is not specified, the default behavior is defi
  name: service
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-grpc-action-schema.json
slug: argo-workflows-io-k8s-api-core-v1-grpc-action
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.GRPCAction
---

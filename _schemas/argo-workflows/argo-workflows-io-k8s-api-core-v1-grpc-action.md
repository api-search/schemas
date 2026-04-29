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
source_filename: argo-workflows-io-k8s-api-core-v1-grpc-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-grpc-action-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.GRPCAction\",\n  \"description\": \"GRPCAction specifies an action involving a GRPC service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"port\": {\n      \"description\": \"Port number of the gRPC service. Number must be in the range 1 to 65535.\",\n      \"type\": \"integer\"\n    },\n    \"service\": {\n      \"description\": \"Service is the name of the service to place in the gRPC HealthCheckRequest (see https://github.com/grpc/grpc/blob/master/doc/health-checking.md).\\n\\nIf this is not specified, the default behavior is defined by gRPC.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"port\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-grpc-action-schema.json
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

---
description: An upstream destination registered with Gloo Gateway, representing a backend service such as a Kubernetes service, static host, AWS Lambda function, or other function provider.
layout: schema
name: Solo.io Gloo Gateway Upstream
properties_list:
- description: Resource metadata including name, namespace, and labels.
  name: metadata
  type: object
- description: Current status of the upstream resource.
  name: status
  type: object
- description: Type of upstream destination.
  name: upstreamType
  type: string
- description: Hostname or address of the upstream.
  name: host
  type: string
- description: Port number of the upstream service.
  name: port
  type: integer
- description: Service specification for function-level routing.
  name: serviceSpec
  type: object
- description: TLS/SSL configuration for the upstream connection.
  name: sslConfig
  type: object
- description: Health check configuration for the upstream.
  name: healthChecks
  type: array
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/upstream.json
slug: upstream
source_filename: upstream.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/upstream.json\",\n  \"title\": \"Solo.io Gloo Gateway Upstream\",\n  \"description\": \"An upstream destination registered with Gloo Gateway, representing a backend service such as a Kubernetes service, static host, AWS Lambda function, or other function provider.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"$ref\": \"resource-metadata.json\",\n      \"description\": \"Resource metadata including name, namespace, and labels.\"\n    },\n    \"status\": {\n      \"$ref\": \"resource-status.json\",\n      \"description\": \"Current status of the upstream resource.\"\n    },\n    \"upstreamType\": {\n      \"type\": \"string\",\n      \"enum\": [\"kube\", \"static\", \"aws\", \"azure\", \"consul\"],\n      \"description\": \"Type of upstream destination.\"\n    },\n    \"host\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Hostname or address of the upstream.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number of the upstream service.\"\n    },\n    \"serviceSpec\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"rest\": {\n          \"type\": \"object\",\n          \"description\": \"REST service specification including discovered functions.\"\n        },\n        \"grpc\": {\n          \"type\": \"object\",\n          \"description\": \"gRPC service specification including discovered services.\"\n        }\n      },\n      \"description\": \"Service specification for function-level routing.\"\n    },\n    \"sslConfig\": {\n      \"type\": \"object\",\n      \"description\": \"TLS/SSL configuration for the upstream connection.\"\n    },\n    \"healthChecks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Health check configuration for the\
  \ upstream.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/upstream.json
tags:
- AI Gateway
- Analytics
- Automation
- Gateways
- Management
- Monetization
- Observability
- Platform
- Resiliency
- Security
- Service Mesh
- Traffic Control
title: Solo.io Gloo Gateway Upstream
---

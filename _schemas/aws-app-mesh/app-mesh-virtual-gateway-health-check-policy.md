---
description: An object that represents the health check policy for a virtual gateway's listener.
layout: schema
name: VirtualGatewayHealthCheckPolicy
properties_list:
- description: ''
  name: healthyThreshold
  type: object
- description: ''
  name: intervalMillis
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: port
  type: object
- description: ''
  name: protocol
  type: object
- description: ''
  name: timeoutMillis
  type: object
- description: ''
  name: unhealthyThreshold
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-health-check-policy-schema.json
slug: app-mesh-virtual-gateway-health-check-policy
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"healthyThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayHealthCheckThreshold\"\n        },\n        {\n          \"description\": \"The number of consecutive successful health checks that must occur before declaring the listener healthy.\"\n        }\n      ]\n    },\n    \"intervalMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayHealthCheckIntervalMillis\"\n        },\n        {\n          \"description\": \"The time period in milliseconds between each health check execution.\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The destination path for the health check request. This value is only used if the specified protocol is HTTP or HTTP/2. For any other protocol, this value is ignored.\"\
  \n        }\n      ]\n    },\n    \"port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The destination port for the health check request. This port must match the port defined in the <a>PortMapping</a> for the listener.\"\n        }\n      ]\n    },\n    \"protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayPortProtocol\"\n        },\n        {\n          \"description\": \"The protocol for the health check request. If you specify <code>grpc</code>, then your service must conform to the <a href=\\\"https://github.com/grpc/grpc/blob/master/doc/health-checking.md\\\">GRPC Health Checking Protocol</a>.\"\n        }\n      ]\n    },\n    \"timeoutMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayHealthCheckTimeoutMillis\"\n        },\n        {\n          \"description\": \"The amount of time\
  \ to wait when receiving a response from the health check, in milliseconds.\"\n        }\n      ]\n    },\n    \"unhealthyThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayHealthCheckThreshold\"\n        },\n        {\n          \"description\": \"The number of consecutive failed health checks that must occur before declaring a virtual gateway unhealthy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"healthyThreshold\",\n    \"intervalMillis\",\n    \"protocol\",\n    \"timeoutMillis\",\n    \"unhealthyThreshold\"\n  ],\n  \"description\": \"An object that represents the health check policy for a virtual gateway's listener.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-health-check-policy-schema.json\",\n  \"title\": \"VirtualGatewayHealthCheckPolicy\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-health-check-policy-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayHealthCheckPolicy
---

---
description: An object that represents the criteria for determining a request match.
layout: schema
name: GrpcGatewayRouteMatch
properties_list:
- description: ''
  name: hostname
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: port
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-gateway-route-match-schema.json
slug: app-mesh-grpc-gateway-route-match
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayRouteHostnameMatch\"\n        },\n        {\n          \"description\": \"The gateway route host name to be matched on.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcGatewayRouteMetadataList\"\n        },\n        {\n          \"description\": \"The gateway route metadata to be matched on.\"\n        }\n      ]\n    },\n    \"port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerPort\"\n        },\n        {\n          \"description\": \"The port number to match from the request.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceName\"\n        },\n        {\n          \"description\": \"The fully qualified domain name for\
  \ the service to match from the request.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the criteria for determining a request match.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-gateway-route-match-schema.json\",\n  \"title\": \"GrpcGatewayRouteMatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-gateway-route-match-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcGatewayRouteMatch
---

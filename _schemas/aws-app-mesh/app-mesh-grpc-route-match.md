---
description: An object that represents the criteria for determining a request match.
layout: schema
name: GrpcRouteMatch
properties_list:
- description: ''
  name: metadata
  type: object
- description: ''
  name: methodName
  type: object
- description: ''
  name: port
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-route-match-schema.json
slug: app-mesh-grpc-route-match
source_filename: app-mesh-grpc-route-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcRouteMetadataList\"\n        },\n        {\n          \"description\": \"An object that represents the data to match from the request.\"\n        }\n      ]\n    },\n    \"methodName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MethodName\"\n        },\n        {\n          \"description\": \"The method name to match from the request. If you specify a name, you must also specify a <code>serviceName</code>.\"\n        }\n      ]\n    },\n    \"port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerPort\"\n        },\n        {\n          \"description\": \"The port number to match on.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceName\"\n        },\n        {\n        \
  \  \"description\": \"The fully qualified domain name for the service to match from the request.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the criteria for determining a request match.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-match-schema.json\",\n  \"title\": \"GrpcRouteMatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-route-match-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcRouteMatch
---

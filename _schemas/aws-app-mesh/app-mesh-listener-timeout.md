---
description: An object that represents timeouts for different protocols.
layout: schema
name: ListenerTimeout
properties_list:
- description: ''
  name: grpc
  type: object
- description: ''
  name: http
  type: object
- description: ''
  name: http2
  type: object
- description: ''
  name: tcp
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-listener-timeout-schema.json
slug: app-mesh-listener-timeout
source_filename: app-mesh-listener-timeout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"grpc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcTimeout\"\n        },\n        {\n          \"description\": \"An object that represents types of timeouts. \"\n        }\n      ]\n    },\n    \"http\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpTimeout\"\n        },\n        {\n          \"description\": \"An object that represents types of timeouts. \"\n        }\n      ]\n    },\n    \"http2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpTimeout\"\n        },\n        {\n          \"description\": \"An object that represents types of timeouts. \"\n        }\n      ]\n    },\n    \"tcp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TcpTimeout\"\n        },\n        {\n          \"description\": \"An object that represents types of timeouts. \"\n        }\n      ]\n    }\n\
  \  },\n  \"description\": \"An object that represents timeouts for different protocols.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-listener-timeout-schema.json\",\n  \"title\": \"ListenerTimeout\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-listener-timeout-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: ListenerTimeout
---

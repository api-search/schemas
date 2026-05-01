---
description: An object that represents types of timeouts.
layout: schema
name: GrpcTimeout
properties_list:
- description: ''
  name: idle
  type: object
- description: ''
  name: perRequest
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-timeout-schema.json
slug: app-mesh-grpc-timeout
source_filename: app-mesh-grpc-timeout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"idle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"An object that represents an idle timeout. An idle timeout bounds the amount of time that a connection may be idle. The default value is none.\"\n        }\n      ]\n    },\n    \"perRequest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"An object that represents a per request timeout. The default value is 15 seconds. If you set a higher timeout, then make sure that the higher value is set for each App Mesh resource in a conversation. For example, if a virtual node backend uses a virtual router provider to route to another virtual node, then the timeout should be greater than 15 seconds for the source and destination virtual node and the route.\"\n        }\n      ]\n    }\n  },\n\
  \  \"description\": \"An object that represents types of timeouts. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-timeout-schema.json\",\n  \"title\": \"GrpcTimeout\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-timeout-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcTimeout
---

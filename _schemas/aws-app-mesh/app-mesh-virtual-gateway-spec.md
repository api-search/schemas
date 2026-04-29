---
description: An object that represents the specification of a service mesh resource.
layout: schema
name: VirtualGatewaySpec
properties_list:
- description: ''
  name: backendDefaults
  type: object
- description: ''
  name: listeners
  type: object
- description: An object that represents logging information.
  name: logging
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-spec-schema.json
slug: app-mesh-virtual-gateway-spec
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"backendDefaults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayBackendDefaults\"\n        },\n        {\n          \"description\": \"A reference to an object that represents the defaults for backends.\"\n        }\n      ]\n    },\n    \"listeners\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayListeners\"\n        },\n        {\n          \"description\": \"The listeners that the mesh endpoint is expected to receive inbound traffic from. You can specify one listener.\"\n        }\n      ]\n    },\n    \"logging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"accessLog\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/VirtualGatewayAccessLog\"\n            },\n            {\n              \"description\": \"The access log configuration.\"\n            }\n         \
  \ ]\n        }\n      },\n      \"description\": \"An object that represents logging information.\"\n    }\n  },\n  \"required\": [\n    \"listeners\"\n  ],\n  \"description\": \"An object that represents the specification of a service mesh resource.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-spec-schema.json\",\n  \"title\": \"VirtualGatewaySpec\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-spec-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewaySpec
---

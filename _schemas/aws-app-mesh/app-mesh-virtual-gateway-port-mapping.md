---
description: An object that represents a port mapping.
layout: schema
name: VirtualGatewayPortMapping
properties_list:
- description: ''
  name: port
  type: object
- description: ''
  name: protocol
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-port-mapping-schema.json
slug: app-mesh-virtual-gateway-port-mapping
source_filename: app-mesh-virtual-gateway-port-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The port used for the port mapping. Specify one protocol.\"\n        }\n      ]\n    },\n    \"protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayPortProtocol\"\n        },\n        {\n          \"description\": \"The protocol used for the port mapping.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"port\",\n    \"protocol\"\n  ],\n  \"description\": \"An object that represents a port mapping.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-port-mapping-schema.json\",\n  \"title\": \"VirtualGatewayPortMapping\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-port-mapping-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayPortMapping
---

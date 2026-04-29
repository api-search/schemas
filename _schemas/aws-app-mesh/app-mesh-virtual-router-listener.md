---
description: An object that represents a virtual router listener.
layout: schema
name: VirtualRouterListener
properties_list:
- description: An object that represents a port mapping.
  name: portMapping
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-router-listener-schema.json
slug: app-mesh-virtual-router-listener
source_filename: app-mesh-virtual-router-listener-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"portMapping\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"port\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PortNumber\"\n            },\n            {\n              \"description\": \"The port used for the port mapping.\"\n            }\n          ]\n        },\n        \"protocol\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PortProtocol\"\n            },\n            {\n              \"description\": \"The protocol used for the port mapping. Specify one protocol.\"\n            }\n          ]\n        }\n      },\n      \"required\": [\n        \"port\",\n        \"protocol\"\n      ],\n      \"description\": \"An object that represents a port mapping.\"\n    }\n  },\n  \"required\": [\n    \"portMapping\"\n  ],\n  \"description\": \"An object that represents a virtual router listener.\",\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-listener-schema.json\",\n  \"title\": \"VirtualRouterListener\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-listener-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualRouterListener
---

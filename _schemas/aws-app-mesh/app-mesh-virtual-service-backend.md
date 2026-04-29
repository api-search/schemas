---
description: An object that represents a virtual service backend for a virtual node.
layout: schema
name: VirtualServiceBackend
properties_list:
- description: ''
  name: clientPolicy
  type: object
- description: ''
  name: virtualServiceName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-service-backend-schema.json
slug: app-mesh-virtual-service-backend
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientPolicy\"\n        },\n        {\n          \"description\": \"A reference to an object that represents the client policy for a backend.\"\n        }\n      ]\n    },\n    \"virtualServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceName\"\n        },\n        {\n          \"description\": \"The name of the virtual service that is acting as a virtual node backend.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualServiceName\"\n  ],\n  \"description\": \"An object that represents a virtual service backend for a virtual node.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-service-backend-schema.json\",\n  \"title\": \"VirtualServiceBackend\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-service-backend-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualServiceBackend
---

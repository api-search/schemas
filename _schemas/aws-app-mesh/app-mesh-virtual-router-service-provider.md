---
description: An object that represents a virtual node service provider.
layout: schema
name: VirtualRouterServiceProvider
properties_list:
- description: ''
  name: virtualRouterName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-router-service-provider-schema.json
slug: app-mesh-virtual-router-service-provider
source_filename: app-mesh-virtual-router-service-provider-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualRouterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the virtual router that is acting as a service provider.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualRouterName\"\n  ],\n  \"description\": \"An object that represents a virtual node service provider.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-service-provider-schema.json\",\n  \"title\": \"VirtualRouterServiceProvider\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-router-service-provider-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualRouterServiceProvider
---

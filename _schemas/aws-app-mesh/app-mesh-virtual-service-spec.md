---
description: An object that represents the specification of a virtual service.
layout: schema
name: VirtualServiceSpec
properties_list:
- description: ''
  name: provider
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-service-spec-schema.json
slug: app-mesh-virtual-service-spec
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualServiceProvider\"\n        },\n        {\n          \"description\": \"The App Mesh object that is acting as the provider for a virtual service. You can specify a single virtual node or virtual router.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the specification of a virtual service.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-service-spec-schema.json\",\n  \"title\": \"VirtualServiceSpec\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-service-spec-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualServiceSpec
---

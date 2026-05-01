---
description: An object that represents the service discovery information for a service mesh.
layout: schema
name: MeshServiceDiscovery
properties_list:
- description: ''
  name: ipPreference
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-mesh-service-discovery-schema.json
slug: app-mesh-mesh-service-discovery
source_filename: app-mesh-mesh-service-discovery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ipPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpPreference\"\n        },\n        {\n          \"description\": \"The IP version to use to control traffic within the mesh.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the service discovery information for a service mesh.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-mesh-service-discovery-schema.json\",\n  \"title\": \"MeshServiceDiscovery\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-mesh-service-discovery-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: MeshServiceDiscovery
---

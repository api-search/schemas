---
description: An object that represents the service discovery information for a virtual node.
layout: schema
name: ServiceDiscovery
properties_list:
- description: ''
  name: awsCloudMap
  type: object
- description: ''
  name: dns
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-service-discovery-schema.json
slug: app-mesh-service-discovery
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsCloudMap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsCloudMapServiceDiscovery\"\n        },\n        {\n          \"description\": \"Specifies any Cloud Map information for the virtual node.\"\n        }\n      ]\n    },\n    \"dns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsServiceDiscovery\"\n        },\n        {\n          \"description\": \"Specifies the DNS information for the virtual node.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the service discovery information for a virtual node.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-service-discovery-schema.json\",\n  \"title\": \"ServiceDiscovery\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-service-discovery-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: ServiceDiscovery
---

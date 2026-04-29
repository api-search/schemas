---
description: An object that represents the DNS service discovery information for your virtual node.
layout: schema
name: DnsServiceDiscovery
properties_list:
- description: ''
  name: hostname
  type: object
- description: ''
  name: ipPreference
  type: object
- description: ''
  name: responseType
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-dns-service-discovery-schema.json
slug: app-mesh-dns-service-discovery
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Hostname\"\n        },\n        {\n          \"description\": \"Specifies the DNS service discovery hostname for the virtual node. \"\n        }\n      ]\n    },\n    \"ipPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpPreference\"\n        },\n        {\n          \"description\": \"The preferred IP version that this virtual node uses. Setting the IP preference on the virtual node only overrides the IP preference set for the mesh on this specific node.\"\n        }\n      ]\n    },\n    \"responseType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsResponseType\"\n        },\n        {\n          \"description\": \"Specifies the DNS response type for the virtual node.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"hostname\"\n  ],\n  \"description\"\
  : \"An object that represents the DNS service discovery information for your virtual node.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-dns-service-discovery-schema.json\",\n  \"title\": \"DnsServiceDiscovery\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-dns-service-discovery-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: DnsServiceDiscovery
---

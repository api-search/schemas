---
description: An object that represents a Transport Layer Security (TLS) client policy.
layout: schema
name: VirtualGatewayClientPolicyTls
properties_list:
- description: ''
  name: certificate
  type: object
- description: ''
  name: enforce
  type: object
- description: ''
  name: ports
  type: object
- description: ''
  name: validation
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualgatewayclientpolicytls-schema.json
slug: amazon-app-mesh-virtualgatewayclientpolicytls
source_filename: amazon-app-mesh-virtualgatewayclientpolicytls-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualGatewayClientPolicyTls\",\n  \"description\": \"An object that represents a Transport Layer Security (TLS) client policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificate\": {},\n    \"enforce\": {},\n    \"ports\": {},\n    \"validation\": {}\n  },\n  \"required\": [\n    \"validation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualgatewayclientpolicytls-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayClientPolicyTls
---

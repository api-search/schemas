---
description: An object that represents a Transport Layer Security (TLS) validation context trust.
layout: schema
name: VirtualGatewayTlsValidationContextTrust
properties_list:
- description: ''
  name: acm
  type: object
- description: ''
  name: file
  type: object
- description: ''
  name: sds
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-tls-validation-context-trust-schema.json
slug: app-mesh-virtual-gateway-tls-validation-context-trust
source_filename: app-mesh-virtual-gateway-tls-validation-context-trust-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"acm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayTlsValidationContextAcmTrust\"\n        },\n        {\n          \"description\": \"A reference to an object that represents a Transport Layer Security (TLS) validation context trust for an Certificate Manager certificate.\"\n        }\n      ]\n    },\n    \"file\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayTlsValidationContextFileTrust\"\n        },\n        {\n          \"description\": \"An object that represents a Transport Layer Security (TLS) validation context trust for a local file.\"\n        }\n      ]\n    },\n    \"sds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayTlsValidationContextSdsTrust\"\n        },\n        {\n          \"description\": \"A reference to an object that represents a virtual gateway's Transport\
  \ Layer Security (TLS) Secret Discovery Service validation context trust.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents a Transport Layer Security (TLS) validation context trust.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-tls-validation-context-trust-schema.json\",\n  \"title\": \"VirtualGatewayTlsValidationContextTrust\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-tls-validation-context-trust-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayTlsValidationContextTrust
---

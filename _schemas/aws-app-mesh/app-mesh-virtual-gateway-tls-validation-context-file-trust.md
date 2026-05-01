---
description: An object that represents a Transport Layer Security (TLS) validation context trust for a local file.
layout: schema
name: VirtualGatewayTlsValidationContextFileTrust
properties_list:
- description: ''
  name: certificateChain
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-tls-validation-context-file-trust-schema.json
slug: app-mesh-virtual-gateway-tls-validation-context-file-trust
source_filename: app-mesh-virtual-gateway-tls-validation-context-file-trust-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateChain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilePath\"\n        },\n        {\n          \"description\": \"The certificate trust chain for a certificate stored on the file system of the virtual node that the proxy is running on.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"certificateChain\"\n  ],\n  \"description\": \"An object that represents a Transport Layer Security (TLS) validation context trust for a local file.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-tls-validation-context-file-trust-schema.json\",\n  \"title\": \"VirtualGatewayTlsValidationContextFileTrust\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-tls-validation-context-file-trust-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayTlsValidationContextFileTrust
---

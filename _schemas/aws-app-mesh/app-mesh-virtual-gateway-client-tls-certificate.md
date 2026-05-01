---
description: An object that represents the virtual gateway's client's Transport Layer Security (TLS) certificate.
layout: schema
name: VirtualGatewayClientTlsCertificate
properties_list:
- description: ''
  name: file
  type: object
- description: ''
  name: sds
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-client-tls-certificate-schema.json
slug: app-mesh-virtual-gateway-client-tls-certificate
source_filename: app-mesh-virtual-gateway-client-tls-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"file\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayListenerTlsFileCertificate\"\n        },\n        {\n          \"description\": \"An object that represents a local file certificate. The certificate must meet specific requirements and you must have proxy authorization enabled. For more information, see <a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html\\\"> Transport Layer Security (TLS) </a>.\"\n        }\n      ]\n    },\n    \"sds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayListenerTlsSdsCertificate\"\n        },\n        {\n          \"description\": \"A reference to an object that represents a virtual gateway's client's Secret Discovery Service certificate.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the virtual gateway's client's Transport Layer Security\
  \ (TLS) certificate.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-client-tls-certificate-schema.json\",\n  \"title\": \"VirtualGatewayClientTlsCertificate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-client-tls-certificate-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayClientTlsCertificate
---

---
description: An object that represents a listener's Transport Layer Security (TLS) certificate.
layout: schema
name: VirtualGatewayListenerTlsCertificate
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
schema_file: json-schema/app-mesh-virtual-gateway-listener-tls-certificate-schema.json
slug: app-mesh-virtual-gateway-listener-tls-certificate
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"acm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayListenerTlsAcmCertificate\"\n        },\n        {\n          \"description\": \"A reference to an object that represents an Certificate Manager certificate.\"\n        }\n      ]\n    },\n    \"file\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayListenerTlsFileCertificate\"\n        },\n        {\n          \"description\": \"A reference to an object that represents a local file certificate.\"\n        }\n      ]\n    },\n    \"sds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayListenerTlsSdsCertificate\"\n        },\n        {\n          \"description\": \"A reference to an object that represents a virtual gateway's listener's Secret Discovery Service certificate.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object\
  \ that represents a listener's Transport Layer Security (TLS) certificate.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listener-tls-certificate-schema.json\",\n  \"title\": \"VirtualGatewayListenerTlsCertificate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listener-tls-certificate-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayListenerTlsCertificate
---

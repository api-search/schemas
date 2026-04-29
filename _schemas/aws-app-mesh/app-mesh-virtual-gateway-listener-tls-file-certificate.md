---
description: An object that represents a local file certificate. The certificate must meet specific requirements and you must have proxy authorization enabled. For more information, see <a href="https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html#virtual-node-tls-prerequisites">Transport Layer Security (TLS)</a>.
layout: schema
name: VirtualGatewayListenerTlsFileCertificate
properties_list:
- description: ''
  name: certificateChain
  type: object
- description: ''
  name: privateKey
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-listener-tls-file-certificate-schema.json
slug: app-mesh-virtual-gateway-listener-tls-file-certificate
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateChain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilePath\"\n        },\n        {\n          \"description\": \"The certificate chain for the certificate.\"\n        }\n      ]\n    },\n    \"privateKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilePath\"\n        },\n        {\n          \"description\": \"The private key for a certificate stored on the file system of the mesh endpoint that the proxy is running on.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"certificateChain\",\n    \"privateKey\"\n  ],\n  \"description\": \"An object that represents a local file certificate. The certificate must meet specific requirements and you must have proxy authorization enabled. For more information, see <a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html#virtual-node-tls-prerequisites\\\">Transport Layer\
  \ Security (TLS)</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listener-tls-file-certificate-schema.json\",\n  \"title\": \"VirtualGatewayListenerTlsFileCertificate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listener-tls-file-certificate-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayListenerTlsFileCertificate
---

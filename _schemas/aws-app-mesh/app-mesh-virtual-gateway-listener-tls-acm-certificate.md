---
description: An object that represents an Certificate Manager certificate.
layout: schema
name: VirtualGatewayListenerTlsAcmCertificate
properties_list:
- description: ''
  name: certificateArn
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-listener-tls-acm-certificate-schema.json
slug: app-mesh-virtual-gateway-listener-tls-acm-certificate
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the certificate. The certificate must meet specific requirements and you must have proxy authorization enabled. For more information, see <a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html#virtual-node-tls-prerequisites\\\">Transport Layer Security (TLS)</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"certificateArn\"\n  ],\n  \"description\": \"An object that represents an Certificate Manager certificate.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listener-tls-acm-certificate-schema.json\",\n  \"title\": \"VirtualGatewayListenerTlsAcmCertificate\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listener-tls-acm-certificate-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayListenerTlsAcmCertificate
---

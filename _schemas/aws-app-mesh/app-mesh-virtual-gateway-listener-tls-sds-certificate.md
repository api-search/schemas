---
description: An object that represents the virtual gateway's listener's Secret Discovery Service certificate.The proxy must be configured with a local SDS provider via a Unix Domain Socket. See App Mesh<a href="https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html">TLS documentation</a> for more info.
layout: schema
name: VirtualGatewayListenerTlsSdsCertificate
properties_list:
- description: ''
  name: secretName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-listener-tls-sds-certificate-schema.json
slug: app-mesh-virtual-gateway-listener-tls-sds-certificate
source_filename: app-mesh-virtual-gateway-listener-tls-sds-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"secretName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewaySdsSecretName\"\n        },\n        {\n          \"description\": \"A reference to an object that represents the name of the secret secret requested from the Secret Discovery Service provider representing Transport Layer Security (TLS) materials like a certificate or certificate chain.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"secretName\"\n  ],\n  \"description\": \"An object that represents the virtual gateway's listener's Secret Discovery Service certificate.The proxy must be configured with a local SDS provider via a Unix Domain Socket. See App Mesh<a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html\\\">TLS documentation</a> for more info. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listener-tls-sds-certificate-schema.json\"\
  ,\n  \"title\": \"VirtualGatewayListenerTlsSdsCertificate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-listener-tls-sds-certificate-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayListenerTlsSdsCertificate
---

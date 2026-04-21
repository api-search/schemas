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
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayListenerTlsFileCertificate
---

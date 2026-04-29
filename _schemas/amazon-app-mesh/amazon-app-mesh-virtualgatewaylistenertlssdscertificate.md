---
description: An object that represents the virtual gateway's listener's Secret Discovery Service certificate.The proxy must be configured with a local SDS provider via a Unix Domain Socket. See App Mesh<a href="https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html">TLS documentation</a> for more info.
layout: schema
name: VirtualGatewayListenerTlsSdsCertificate
properties_list:
- description: ''
  name: secretName
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualgatewaylistenertlssdscertificate-schema.json
slug: amazon-app-mesh-virtualgatewaylistenertlssdscertificate
source_filename: amazon-app-mesh-virtualgatewaylistenertlssdscertificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualGatewayListenerTlsSdsCertificate\",\n  \"description\": \"An object that represents the virtual gateway's listener's Secret Discovery Service certificate.The proxy must be configured with a local SDS provider via a Unix Domain Socket. See App Mesh<a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html\\\">TLS documentation</a> for more info. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"secretName\": {}\n  },\n  \"required\": [\n    \"secretName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualgatewaylistenertlssdscertificate-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayListenerTlsSdsCertificate
---

---
description: An object that represents a virtual gateway's listener's Transport Layer Security (TLS) validation context.
layout: schema
name: VirtualGatewayListenerTlsValidationContext
properties_list:
- description: ''
  name: subjectAlternativeNames
  type: object
- description: ''
  name: trust
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualgatewaylistenertlsvalidationcontext-schema.json
slug: amazon-app-mesh-virtualgatewaylistenertlsvalidationcontext
source_filename: amazon-app-mesh-virtualgatewaylistenertlsvalidationcontext-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualGatewayListenerTlsValidationContext\",\n  \"description\": \"An object that represents a virtual gateway's listener's Transport Layer Security (TLS) validation context.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subjectAlternativeNames\": {},\n    \"trust\": {}\n  },\n  \"required\": [\n    \"trust\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualgatewaylistenertlsvalidationcontext-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayListenerTlsValidationContext
---

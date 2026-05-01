---
description: An object that represents a Transport Layer Security (TLS) validation context.
layout: schema
name: VirtualGatewayTlsValidationContext
properties_list:
- description: ''
  name: subjectAlternativeNames
  type: object
- description: ''
  name: trust
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-virtualgatewaytlsvalidationcontext-schema.json
slug: amazon-app-mesh-virtualgatewaytlsvalidationcontext
source_filename: amazon-app-mesh-virtualgatewaytlsvalidationcontext-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VirtualGatewayTlsValidationContext\",\n  \"description\": \"An object that represents a Transport Layer Security (TLS) validation context.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subjectAlternativeNames\": {},\n    \"trust\": {}\n  },\n  \"required\": [\n    \"trust\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-virtualgatewaytlsvalidationcontext-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayTlsValidationContext
---

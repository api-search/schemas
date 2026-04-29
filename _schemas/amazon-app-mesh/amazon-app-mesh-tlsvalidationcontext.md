---
description: An object that represents how the proxy will validate its peer during Transport Layer Security (TLS) negotiation.
layout: schema
name: TlsValidationContext
properties_list:
- description: ''
  name: subjectAlternativeNames
  type: object
- description: ''
  name: trust
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-tlsvalidationcontext-schema.json
slug: amazon-app-mesh-tlsvalidationcontext
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TlsValidationContext\",\n  \"description\": \"An object that represents how the proxy will validate its peer during Transport Layer Security (TLS) negotiation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subjectAlternativeNames\": {},\n    \"trust\": {}\n  },\n  \"required\": [\n    \"trust\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-tlsvalidationcontext-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: TlsValidationContext
---

---
description: A gateway resource that defines listeners and bind addresses used by Envoy to accept incoming connections in Gloo Gateway.
layout: schema
name: Solo.io Gloo Gateway
properties_list:
- description: Resource metadata including name, namespace, and labels.
  name: metadata
  type: object
- description: Current status of the gateway resource.
  name: status
  type: object
- description: Address the gateway listens on.
  name: bindAddress
  type: string
- description: Port the gateway listens on.
  name: bindPort
  type: integer
- description: Whether SSL/TLS is enabled on this gateway.
  name: ssl
  type: boolean
- description: HTTP gateway configuration.
  name: httpGateway
  type: object
- description: TCP gateway configuration.
  name: tcpGateway
  type: object
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/gateway.json
slug: gateway
source_filename: gateway.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/gateway.json\",\n  \"title\": \"Solo.io Gloo Gateway\",\n  \"description\": \"A gateway resource that defines listeners and bind addresses used by Envoy to accept incoming connections in Gloo Gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"$ref\": \"resource-metadata.json\",\n      \"description\": \"Resource metadata including name, namespace, and labels.\"\n    },\n    \"status\": {\n      \"$ref\": \"resource-status.json\",\n      \"description\": \"Current status of the gateway resource.\"\n    },\n    \"bindAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Address the gateway listens on.\"\n    },\n    \"bindPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Port the gateway listens on.\"\n    },\n    \"ssl\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether SSL/TLS is enabled on this gateway.\"\n    },\n    \"httpGateway\": {\n      \"type\": \"object\",\n      \"description\": \"HTTP gateway configuration.\"\n    },\n    \"tcpGateway\": {\n      \"type\": \"object\",\n      \"description\": \"TCP gateway configuration.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/gateway.json
tags:
- AI Gateway
- Analytics
- Automation
- Gateways
- Management
- Monetization
- Observability
- Platform
- Resiliency
- Security
- Service Mesh
- Traffic Control
title: Solo.io Gloo Gateway
---

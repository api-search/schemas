---
description: A TLS Edge defines a TLS endpoint with TLS termination, mutual TLS, backend, and IP restriction configurations.
layout: schema
name: ngrok TLS Edge
properties_list:
- description: Unique identifier for the TLS edge.
  name: id
  type: string
- description: Human-readable description of the edge.
  name: description
  type: string
- description: Arbitrary user-defined metadata.
  name: metadata
  type: string
- description: Timestamp when the edge was created.
  name: created_at
  type: string
- description: URI of the edge API resource.
  name: uri
  type: string
- description: The host:port combinations that this edge listens on.
  name: hostports
  type: array
- description: The backend configuration for the TLS edge.
  name: backend
  type: object
- description: The IP restriction module configuration.
  name: ip_restriction
  type: object
- description: The mutual TLS module configuration.
  name: mutual_tls
  type: object
- description: The TLS termination module configuration.
  name: tls_termination
  type: object
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/tls-edge.json
slug: tls-edge
source_filename: tls-edge.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/tls-edge.json\",\n  \"title\": \"ngrok TLS Edge\",\n  \"description\": \"A TLS Edge defines a TLS endpoint with TLS termination, mutual TLS, backend, and IP restriction configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the TLS edge.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the edge.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined metadata.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the edge was created.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the edge\
  \ API resource.\"\n    },\n    \"hostports\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The host:port combinations that this edge listens on.\"\n    },\n    \"backend\": {\n      \"type\": \"object\",\n      \"description\": \"The backend configuration for the TLS edge.\"\n    },\n    \"ip_restriction\": {\n      \"type\": \"object\",\n      \"description\": \"The IP restriction module configuration.\"\n    },\n    \"mutual_tls\": {\n      \"type\": \"object\",\n      \"description\": \"The mutual TLS module configuration.\"\n    },\n    \"tls_termination\": {\n      \"type\": \"object\",\n      \"description\": \"The TLS termination module configuration.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/tls-edge.json
tags:
- AI Gateway
- API Gateway
- Compute
- Developer Tools
- Gateways
- Ingress
- Platform
- Proxies
- Servers
- Tunnels
title: ngrok TLS Edge
---

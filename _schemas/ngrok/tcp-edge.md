---
description: A TCP Edge defines a TCP endpoint for non-HTTP protocols with backend and IP restriction configurations.
layout: schema
name: ngrok TCP Edge
properties_list:
- description: Unique identifier for the TCP edge.
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
- description: The backend configuration for the TCP edge.
  name: backend
  type: object
- description: The IP restriction module configuration.
  name: ip_restriction
  type: object
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/tcp-edge.json
slug: tcp-edge
source_filename: tcp-edge.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/tcp-edge.json\",\n  \"title\": \"ngrok TCP Edge\",\n  \"description\": \"A TCP Edge defines a TCP endpoint for non-HTTP protocols with backend and IP restriction configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the TCP edge.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the edge.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined metadata.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the edge was created.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the edge API resource.\"\
  \n    },\n    \"hostports\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The host:port combinations that this edge listens on.\"\n    },\n    \"backend\": {\n      \"type\": \"object\",\n      \"description\": \"The backend configuration for the TCP edge.\"\n    },\n    \"ip_restriction\": {\n      \"type\": \"object\",\n      \"description\": \"The IP restriction module configuration.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/tcp-edge.json
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
title: ngrok TCP Edge
---

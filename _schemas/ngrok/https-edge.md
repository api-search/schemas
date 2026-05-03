---
description: An HTTPS Edge defines an HTTPS endpoint with routes and modules that can be configured for traffic management, authentication, and other policies.
layout: schema
name: ngrok HTTPS Edge
properties_list:
- description: Unique identifier for the HTTPS edge.
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
- description: The routes associated with this HTTPS edge.
  name: routes
  type: array
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/https-edge.json
slug: https-edge
source_filename: https-edge.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/https-edge.json\",\n  \"title\": \"ngrok HTTPS Edge\",\n  \"description\": \"An HTTPS Edge defines an HTTPS endpoint with routes and modules that can be configured for traffic management, authentication, and other policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the HTTPS edge.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the edge.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined metadata.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the edge was created.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"URI of the edge API resource.\"\n    },\n    \"hostports\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The host:port combinations that this edge listens on.\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"The routes associated with this HTTPS edge.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/https-edge.json
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
title: ngrok HTTPS Edge
---

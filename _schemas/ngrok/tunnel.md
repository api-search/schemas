---
description: A Tunnel represents an individual tunnel connection within a tunnel session, exposing a local service via a public URL through the ngrok network.
layout: schema
name: ngrok Tunnel
properties_list:
- description: Unique identifier for the tunnel.
  name: id
  type: string
- description: The public URL of the tunnel.
  name: public_url
  type: string
- description: Timestamp when the tunnel was started.
  name: started_at
  type: string
- description: Arbitrary user-defined metadata for the tunnel.
  name: metadata
  type: string
- description: The protocol of the tunnel (e.g., http, https, tcp, tls).
  name: proto
  type: string
- description: The ngrok region where the tunnel is running.
  name: region
  type: string
- description: Reference to the tunnel session that created this tunnel.
  name: tunnel_session
  type: object
- description: Reference to the endpoint associated with this tunnel.
  name: endpoint
  type: object
- description: Labels assigned to the tunnel for routing with labeled tunnels.
  name: labels
  type: object
- description: References to the backends this tunnel is attached to.
  name: backends
  type: array
- description: The address that this tunnel forwards traffic to.
  name: forwards_to
  type: string
- description: URI of the tunnel API resource.
  name: uri
  type: string
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/tunnel.json
slug: tunnel
source_filename: tunnel.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/tunnel.json\",\n  \"title\": \"ngrok Tunnel\",\n  \"description\": \"A Tunnel represents an individual tunnel connection within a tunnel session, exposing a local service via a public URL through the ngrok network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the tunnel.\"\n    },\n    \"public_url\": {\n      \"type\": \"string\",\n      \"description\": \"The public URL of the tunnel.\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the tunnel was started.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined metadata for the tunnel.\"\n    },\n    \"proto\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"The protocol of the tunnel (e.g., http, https, tcp, tls).\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The ngrok region where the tunnel is running.\"\n    },\n    \"tunnel_session\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the tunnel session that created this tunnel.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"uri\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"endpoint\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the endpoint associated with this tunnel.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"uri\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels assigned to\
  \ the tunnel for routing with labeled tunnels.\"\n    },\n    \"backends\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"uri\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"References to the backends this tunnel is attached to.\"\n    },\n    \"forwards_to\": {\n      \"type\": \"string\",\n      \"description\": \"The address that this tunnel forwards traffic to.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the tunnel API resource.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/tunnel.json
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
title: ngrok Tunnel
---

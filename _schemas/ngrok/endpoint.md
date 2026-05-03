---
description: An Endpoint represents a public URL that routes traffic to a tunnel or edge configuration in the ngrok network.
layout: schema
name: ngrok Endpoint
properties_list:
- description: Unique identifier for the endpoint.
  name: id
  type: string
- description: The ngrok region where the endpoint is hosted.
  name: region
  type: string
- description: Timestamp when the endpoint was created.
  name: created_at
  type: string
- description: Timestamp when the endpoint was last updated.
  name: updated_at
  type: string
- description: The public URL of the endpoint.
  name: public_url
  type: string
- description: The protocol of the endpoint (http, https, tcp, tls).
  name: proto
  type: string
- description: The URL of the endpoint.
  name: url
  type: string
- description: The type of the endpoint (ephemeral, edge, cloud).
  name: type
  type: string
- description: Human-readable description of the endpoint.
  name: description
  type: string
- description: Arbitrary user-defined metadata.
  name: metadata
  type: string
- description: Reference to the reserved domain, if applicable.
  name: domain
  type: object
- description: Reference to the reserved TCP address, if applicable.
  name: tcp_addr
  type: object
- description: Reference to the tunnel serving this endpoint.
  name: tunnel
  type: object
- description: Reference to the edge serving this endpoint.
  name: edge
  type: object
- description: The bindings for the endpoint.
  name: bindings
  type: array
- description: The traffic policy attached to this endpoint.
  name: traffic_policy
  type: string
- description: URI of the endpoint API resource.
  name: uri
  type: string
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/endpoint.json
slug: endpoint
source_filename: endpoint.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/endpoint.json\",\n  \"title\": \"ngrok Endpoint\",\n  \"description\": \"An Endpoint represents a public URL that routes traffic to a tunnel or edge configuration in the ngrok network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the endpoint.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The ngrok region where the endpoint is hosted.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the endpoint was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the endpoint was last updated.\"\n    },\n    \"public_url\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The public URL of the endpoint.\"\n    },\n    \"proto\": {\n      \"type\": \"string\",\n      \"description\": \"The protocol of the endpoint (http, https, tcp, tls).\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the endpoint.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the endpoint (ephemeral, edge, cloud).\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the endpoint.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined metadata.\"\n    },\n    \"domain\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the reserved domain, if applicable.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"uri\": {\n          \"type\": \"string\"\n        }\n     \
  \ }\n    },\n    \"tcp_addr\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the reserved TCP address, if applicable.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"uri\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"tunnel\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the tunnel serving this endpoint.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"uri\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"edge\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the edge serving this endpoint.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"uri\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"bindings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n\
  \      \"description\": \"The bindings for the endpoint.\"\n    },\n    \"traffic_policy\": {\n      \"type\": \"string\",\n      \"description\": \"The traffic policy attached to this endpoint.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the endpoint API resource.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/endpoint.json
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
title: ngrok Endpoint
---

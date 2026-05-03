---
description: A Tunnel Session represents a running ngrok agent connection to the ngrok service.
layout: schema
name: ngrok Tunnel Session
properties_list:
- description: Unique identifier for the tunnel session.
  name: id
  type: string
- description: URI of the tunnel session API resource.
  name: uri
  type: string
- description: The version of the ngrok agent.
  name: agent_version
  type: string
- description: Reference to the credential used to authenticate the session.
  name: credential
  type: object
- description: The IP address of the agent.
  name: ip
  type: string
- description: Arbitrary user-defined metadata.
  name: metadata
  type: string
- description: The operating system of the agent host.
  name: os
  type: string
- description: The ngrok region the session is connected to.
  name: region
  type: string
- description: Timestamp when the session started.
  name: started_at
  type: string
- description: The transport protocol used for the session.
  name: transport
  type: string
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/tunnel-session.json
slug: tunnel-session
source_filename: tunnel-session.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/tunnel-session.json\",\n  \"title\": \"ngrok Tunnel Session\",\n  \"description\": \"A Tunnel Session represents a running ngrok agent connection to the ngrok service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the tunnel session.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the tunnel session API resource.\"\n    },\n    \"agent_version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the ngrok agent.\"\n    },\n    \"credential\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the credential used to authenticate the session.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"uri\": {\n        \
  \  \"type\": \"string\"\n        }\n      }\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address of the agent.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined metadata.\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system of the agent host.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The ngrok region the session is connected to.\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the session started.\"\n    },\n    \"transport\": {\n      \"type\": \"string\",\n      \"description\": \"The transport protocol used for the session.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/tunnel-session.json
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
title: ngrok Tunnel Session
---

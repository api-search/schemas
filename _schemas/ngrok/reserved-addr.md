---
description: A Reserved Address is a static TCP address reserved for use with TCP tunnels.
layout: schema
name: ngrok Reserved Address
properties_list:
- description: Unique identifier for the reserved address.
  name: id
  type: string
- description: URI of the reserved address API resource.
  name: uri
  type: string
- description: Timestamp when the reserved address was created.
  name: created_at
  type: string
- description: Human-readable description.
  name: description
  type: string
- description: Arbitrary user-defined metadata.
  name: metadata
  type: string
- description: The reserved TCP address in host:port format.
  name: addr
  type: string
- description: The ngrok region where the address is reserved.
  name: region
  type: string
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/reserved-addr.json
slug: reserved-addr
source_filename: reserved-addr.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/reserved-addr.json\",\n  \"title\": \"ngrok Reserved Address\",\n  \"description\": \"A Reserved Address is a static TCP address reserved for use with TCP tunnels.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the reserved address.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the reserved address API resource.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the reserved address was created.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined\
  \ metadata.\"\n    },\n    \"addr\": {\n      \"type\": \"string\",\n      \"description\": \"The reserved TCP address in host:port format.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The ngrok region where the address is reserved.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/reserved-addr.json
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
title: ngrok Reserved Address
---

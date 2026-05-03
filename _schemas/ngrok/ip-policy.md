---
description: An IP Policy contains rules to allow or deny traffic from specific IP address ranges.
layout: schema
name: ngrok IP Policy
properties_list:
- description: Unique identifier for the IP policy.
  name: id
  type: string
- description: URI of the IP policy API resource.
  name: uri
  type: string
- description: Timestamp when the IP policy was created.
  name: created_at
  type: string
- description: Human-readable description.
  name: description
  type: string
- description: Arbitrary user-defined metadata.
  name: metadata
  type: string
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/ip-policy.json
slug: ip-policy
source_filename: ip-policy.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/ip-policy.json\",\n  \"title\": \"ngrok IP Policy\",\n  \"description\": \"An IP Policy contains rules to allow or deny traffic from specific IP address ranges.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the IP policy.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the IP policy API resource.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the IP policy was created.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined metadata.\"\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/ip-policy.json
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
title: ngrok IP Policy
---

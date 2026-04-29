---
description: An intention authorizes or denies traffic between two services in the Consul service mesh.
layout: schema
name: Consul Connect Intention
properties_list:
- description: Server-assigned UUID (deprecated in v1.9+ in favor of source/destination addressing).
  name: ID
  type: string
- description: Source service name. Use '*' for any source.
  name: SourceName
  type: string
- description: Destination service name.
  name: DestinationName
  type: string
- description: Source namespace (Consul Enterprise).
  name: SourceNS
  type: string
- description: Destination namespace (Consul Enterprise).
  name: DestinationNS
  type: string
- description: Whether the intention permits or denies the connection.
  name: Action
  type: string
- description: Human-readable description of the intention.
  name: Description
  type: string
- description: Server-computed precedence used to evaluate overlapping intentions.
  name: Precedence
  type: integer
- description: Arbitrary key/value metadata.
  name: Meta
  type: object
provider_name: Consul Connect
provider_slug: consul-connect
schema_file: json-schema/consul-connect-intention-schema.json
slug: consul-connect-intention
source_filename: consul-connect-intention-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.hashicorp.com/consul/schemas/intention.json\",\n  \"title\": \"Consul Connect Intention\",\n  \"description\": \"An intention authorizes or denies traffic between two services in the Consul service mesh.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"type\": \"string\",\n      \"description\": \"Server-assigned UUID (deprecated in v1.9+ in favor of source/destination addressing).\"\n    },\n    \"SourceName\": {\n      \"type\": \"string\",\n      \"description\": \"Source service name. Use '*' for any source.\"\n    },\n    \"DestinationName\": {\n      \"type\": \"string\",\n      \"description\": \"Destination service name.\"\n    },\n    \"SourceNS\": {\n      \"type\": \"string\",\n      \"description\": \"Source namespace (Consul Enterprise).\"\n    },\n    \"DestinationNS\": {\n      \"type\": \"string\",\n      \"description\": \"Destination\
  \ namespace (Consul Enterprise).\"\n    },\n    \"Action\": {\n      \"type\": \"string\",\n      \"enum\": [\"allow\", \"deny\"],\n      \"description\": \"Whether the intention permits or denies the connection.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the intention.\"\n    },\n    \"Precedence\": {\n      \"type\": \"integer\",\n      \"description\": \"Server-computed precedence used to evaluate overlapping intentions.\"\n    },\n    \"Meta\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary key/value metadata.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    }\n  },\n  \"required\": [\"SourceName\", \"DestinationName\", \"Action\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/consul-connect/refs/heads/main/json-schema/consul-connect-intention-schema.json
tags:
- Consul
- Envoy
- HashiCorp
- Intentions
- Kubernetes
- mTLS
- Service Mesh
- Sidecar
- Zero Trust
title: Consul Connect Intention
---

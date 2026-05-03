---
description: A proxy resource representing the compiled Envoy configuration generated from virtual services, upstreams, and other gateway resources.
layout: schema
name: Solo.io Gloo Gateway Proxy
properties_list:
- description: Resource metadata including name, namespace, and labels.
  name: metadata
  type: object
- description: Current status of the proxy resource.
  name: status
  type: object
- description: List of listeners configured on this proxy.
  name: listeners
  type: array
- description: Compressed representation of the full proxy specification.
  name: compressedSpec
  type: string
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/proxy.json
slug: proxy
source_filename: proxy.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/proxy.json\",\n  \"title\": \"Solo.io Gloo Gateway Proxy\",\n  \"description\": \"A proxy resource representing the compiled Envoy configuration generated from virtual services, upstreams, and other gateway resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"$ref\": \"resource-metadata.json\",\n      \"description\": \"Resource metadata including name, namespace, and labels.\"\n    },\n    \"status\": {\n      \"$ref\": \"resource-status.json\",\n      \"description\": \"Current status of the proxy resource.\"\n    },\n    \"listeners\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"List of listeners configured on this proxy.\"\n    },\n    \"compressedSpec\": {\n      \"type\": \"string\",\n      \"description\": \"Compressed\
  \ representation of the full proxy specification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/proxy.json
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
title: Solo.io Gloo Gateway Proxy
---

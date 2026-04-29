---
description: An Ambassador TLSContext resource that configures TLS settings for inbound or outbound connections, including certificates, protocols, and cipher suites.
layout: schema
name: TLSContext
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-tls-context-schema.json
slug: ambassador-tls-context
source_filename: ambassador-tls-context-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TLSContext\",\n  \"type\": \"object\",\n  \"description\": \"An Ambassador TLSContext resource that configures TLS settings for inbound or outbound connections, including certificates, protocols, and cipher suites.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-tls-context-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: TLSContext
---

---
description: An Ambassador Host resource that configures how Ambassador handles requests for a specific hostname, including TLS termination and ACME certificate management.
layout: schema
name: Host
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-host-schema.json
slug: ambassador-host
source_filename: ambassador-host-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Host\",\n  \"type\": \"object\",\n  \"description\": \"An Ambassador Host resource that configures how Ambassador handles requests for a specific hostname, including TLS termination and ACME certificate management.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-host-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: Host
---

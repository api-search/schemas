---
description: Specification for an Ambassador Host
layout: schema
name: HostSpec
properties_list:
- description: Hostname that this Host resource applies to. Supports wildcard patterns like *.example.com.
  name: hostname
  type: string
- description: Ambassador IDs that should apply this Host
  name: ambassador_id
  type: array
- description: ACME certificate provider configuration for automatic TLS certificates
  name: acmeProvider
  type: object
- description: Reference to a TLSContext resource for TLS configuration
  name: tlsContext
  type: object
- description: Reference to a Kubernetes TLS Secret containing certificates
  name: tlsSecret
  type: object
- description: Policy for handling insecure requests
  name: requestPolicy
  type: object
- description: Label selector for Mappings this Host should be associated with
  name: selector
  type: object
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-host-spec-schema.json
slug: ambassador-host-spec
source_filename: ambassador-host-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HostSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for an Ambassador Host\",\n  \"properties\": {\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname that this Host resource applies to. Supports wildcard patterns like *.example.com.\"\n    },\n    \"ambassador_id\": {\n      \"type\": \"array\",\n      \"description\": \"Ambassador IDs that should apply this Host\"\n    },\n    \"acmeProvider\": {\n      \"type\": \"object\",\n      \"description\": \"ACME certificate provider configuration for automatic TLS certificates\"\n    },\n    \"tlsContext\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a TLSContext resource for TLS configuration\"\n    },\n    \"tlsSecret\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a Kubernetes TLS Secret containing certificates\"\n    },\n    \"requestPolicy\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Policy for handling insecure requests\"\n    },\n    \"selector\": {\n      \"type\": \"object\",\n      \"description\": \"Label selector for Mappings this Host should be associated with\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-host-spec-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: HostSpec
---

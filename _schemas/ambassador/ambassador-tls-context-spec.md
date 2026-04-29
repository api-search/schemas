---
description: Specification for a TLSContext resource
layout: schema
name: TLSContextSpec
properties_list:
- description: Hostnames this TLSContext applies to
  name: hosts
  type: array
- description: Name of the Kubernetes Secret containing TLS certificates
  name: secret
  type: string
- description: Path to the certificate chain PEM file (alternative to secret)
  name: cert_chain_file
  type: string
- description: Path to the private key PEM file (alternative to secret)
  name: private_key_file
  type: string
- description: Name of the Kubernetes Secret containing CA certificates for client verification
  name: ca_secret
  type: string
- description: Whether client TLS certificates are required (mTLS)
  name: cert_required
  type: boolean
- description: Minimum TLS version to accept
  name: min_tls_version
  type: string
- description: Maximum TLS version to accept
  name: max_tls_version
  type: string
- description: Allowed TLS cipher suites
  name: cipher_suites
  type: array
- description: Allowed ECDH curves
  name: ecdh_curves
  type: array
- description: ALPN protocols to advertise
  name: alpn_protocols
  type: string
- description: Port number from which to redirect cleartext traffic to TLS
  name: redirect_cleartext_from
  type: integer
- description: SNI hostname to present for outbound TLS connections
  name: sni
  type: string
- description: Ambassador IDs that should use this TLSContext
  name: ambassador_id
  type: array
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-tls-context-spec-schema.json
slug: ambassador-tls-context-spec
source_filename: ambassador-tls-context-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TLSContextSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for a TLSContext resource\",\n  \"properties\": {\n    \"hosts\": {\n      \"type\": \"array\",\n      \"description\": \"Hostnames this TLSContext applies to\"\n    },\n    \"secret\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Kubernetes Secret containing TLS certificates\"\n    },\n    \"cert_chain_file\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the certificate chain PEM file (alternative to secret)\"\n    },\n    \"private_key_file\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the private key PEM file (alternative to secret)\"\n    },\n    \"ca_secret\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Kubernetes Secret containing CA certificates for client verification\"\n    },\n    \"cert_required\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether client TLS certificates are required (mTLS)\"\n    },\n    \"min_tls_version\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum TLS version to accept\"\n    },\n    \"max_tls_version\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum TLS version to accept\"\n    },\n    \"cipher_suites\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed TLS cipher suites\"\n    },\n    \"ecdh_curves\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed ECDH curves\"\n    },\n    \"alpn_protocols\": {\n      \"type\": \"string\",\n      \"description\": \"ALPN protocols to advertise\"\n    },\n    \"redirect_cleartext_from\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number from which to redirect cleartext traffic to TLS\"\n    },\n    \"sni\": {\n      \"type\": \"string\",\n      \"description\": \"SNI hostname to present for outbound TLS connections\"\n    },\n    \"ambassador_id\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Ambassador IDs that should use this TLSContext\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-tls-context-spec-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: TLSContextSpec
---

---
description: TLS configuration for enabling HTTPS on the KrakenD API Gateway, including certificate paths, minimum TLS version, and cipher suite preferences.
layout: schema
name: KrakenD TLS Configuration
properties_list:
- description: Path to the public key or certificate PEM file.
  name: public_key
  type: string
- description: Path to the private key PEM file.
  name: private_key
  type: string
- description: Minimum TLS version accepted.
  name: min_version
  type: string
- description: Maximum TLS version accepted.
  name: max_version
  type: string
- description: Elliptic curve preferences for TLS handshake.
  name: curve_preferences
  type: array
- description: Whether to prefer the server cipher suite order.
  name: prefer_server_cipher_suites
  type: boolean
- description: List of supported cipher suite IDs.
  name: cipher_suites
  type: array
- description: Disables TLS even when certificate files are present.
  name: disabled
  type: boolean
- description: Enables mutual TLS authentication.
  name: enable_mtls
  type: boolean
- description: Paths to CA certificate files for mTLS client verification.
  name: ca_certs
  type: array
provider_name: KrakenD
provider_slug: krakend
schema_file: json-schema/tls.json
slug: tls
source_filename: tls.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/krakend/blob/main/json-schema/tls.json\",\n  \"title\": \"KrakenD TLS Configuration\",\n  \"description\": \"TLS configuration for enabling HTTPS on the KrakenD API Gateway, including certificate paths, minimum TLS version, and cipher suite preferences.\",\n  \"type\": \"object\",\n  \"required\": [\"public_key\", \"private_key\"],\n  \"properties\": {\n    \"public_key\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the public key or certificate PEM file.\"\n    },\n    \"private_key\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the private key PEM file.\"\n    },\n    \"min_version\": {\n      \"type\": \"string\",\n      \"enum\": [\"SSL3.0\", \"TLS10\", \"TLS11\", \"TLS12\", \"TLS13\"],\n      \"description\": \"Minimum TLS version accepted.\"\n    },\n    \"max_version\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\"SSL3.0\", \"TLS10\", \"TLS11\", \"TLS12\", \"TLS13\"],\n      \"description\": \"Maximum TLS version accepted.\"\n    },\n    \"curve_preferences\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"Elliptic curve preferences for TLS handshake.\"\n    },\n    \"prefer_server_cipher_suites\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to prefer the server cipher suite order.\"\n    },\n    \"cipher_suites\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"List of supported cipher suite IDs.\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Disables TLS even when certificate files are present.\"\n    },\n    \"enable_mtls\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Enables mutual TLS authentication.\"\n    },\n    \"ca_certs\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Paths to CA certificate files for mTLS client verification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/krakend/refs/heads/main/json-schema/tls.json
tags:
- Aggregation
- API Gateway
- Go
- Open Source
title: KrakenD TLS Configuration
---

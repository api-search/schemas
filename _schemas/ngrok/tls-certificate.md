---
description: A TLS Certificate is an x509 certificate and private key pair used to terminate TLS traffic on ngrok endpoints.
layout: schema
name: ngrok TLS Certificate
properties_list:
- description: Unique identifier for the TLS certificate.
  name: id
  type: string
- description: URI of the TLS certificate API resource.
  name: uri
  type: string
- description: Timestamp when the certificate was uploaded.
  name: created_at
  type: string
- description: Human-readable description.
  name: description
  type: string
- description: Arbitrary user-defined metadata.
  name: metadata
  type: string
- description: The PEM-encoded certificate chain.
  name: certificate_pem
  type: string
- description: The subject common name from the certificate.
  name: subject_common_name
  type: string
- description: Subject alternative names from the certificate.
  name: subject_alternative_names
  type: object
- description: The certificate is not valid before this time.
  name: not_before
  type: string
- description: The certificate is not valid after this time.
  name: not_after
  type: string
- description: Key usage extensions from the certificate.
  name: key_usages
  type: array
- description: Extended key usage extensions from the certificate.
  name: extended_key_usages
  type: array
- description: The type of the private key (rsa, ecdsa, ed25519).
  name: private_key_type
  type: string
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/tls-certificate.json
slug: tls-certificate
source_filename: tls-certificate.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/tls-certificate.json\",\n  \"title\": \"ngrok TLS Certificate\",\n  \"description\": \"A TLS Certificate is an x509 certificate and private key pair used to terminate TLS traffic on ngrok endpoints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the TLS certificate.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the TLS certificate API resource.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the certificate was uploaded.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Arbitrary user-defined metadata.\"\n    },\n    \"certificate_pem\": {\n      \"type\": \"string\",\n      \"description\": \"The PEM-encoded certificate chain.\"\n    },\n    \"subject_common_name\": {\n      \"type\": \"string\",\n      \"description\": \"The subject common name from the certificate.\"\n    },\n    \"subject_alternative_names\": {\n      \"type\": \"object\",\n      \"description\": \"Subject alternative names from the certificate.\",\n      \"properties\": {\n        \"dns_names\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"DNS name SANs.\"\n        },\n        \"ips\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"IP address SANs.\"\n        }\n      }\n    },\n    \"not_before\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The certificate\
  \ is not valid before this time.\"\n    },\n    \"not_after\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The certificate is not valid after this time.\"\n    },\n    \"key_usages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key usage extensions from the certificate.\"\n    },\n    \"extended_key_usages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Extended key usage extensions from the certificate.\"\n    },\n    \"private_key_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the private key (rsa, ecdsa, ed25519).\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/tls-certificate.json
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
title: ngrok TLS Certificate
---

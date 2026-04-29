---
description: A Certificate object represents a public certificate for TLS termination.
layout: schema
name: Certificate
properties_list:
- description: ''
  name: id
  type: string
- description: PEM-encoded public certificate chain.
  name: cert
  type: string
- description: PEM-encoded private key of the certificate.
  name: key
  type: string
- description: PEM-encoded public certificate chain of the alternate certificate.
  name: cert_alt
  type: string
- description: PEM-encoded private key of the alternate certificate.
  name: key_alt
  type: string
- description: The list of SNI hostnames associated with this certificate.
  name: snis
  type: array
- description: ''
  name: tags
  type: array
- description: ''
  name: created_at
  type: integer
- description: ''
  name: updated_at
  type: integer
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-certificate-schema.json
slug: kong-gateway-admin-certificate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Certificate\",\n  \"type\": \"object\",\n  \"description\": \"A Certificate object represents a public certificate for TLS termination.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"cert\": {\n      \"type\": \"string\",\n      \"description\": \"PEM-encoded public certificate chain.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"PEM-encoded private key of the certificate.\"\n    },\n    \"cert_alt\": {\n      \"type\": \"string\",\n      \"description\": \"PEM-encoded public certificate chain of the alternate certificate.\"\n    },\n    \"key_alt\": {\n      \"type\": \"string\",\n      \"description\": \"PEM-encoded private key of the alternate certificate.\"\n    },\n    \"snis\": {\n      \"type\": \"array\",\n      \"description\": \"The list of SNI hostnames associated with this certificate.\"\n    },\n    \"tags\":\
  \ {\n      \"type\": \"array\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-certificate-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: Certificate
---

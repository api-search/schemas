---
description: As of http://tools.ietf.org/html/draft-ietf-jose-json-web-key-18.
layout: schema
name: JsonWebKey
properties_list:
- description: Key identifier.
  name: kid
  type: string
- description: Supported key operations.
  name: key_ops
  type: array
- description: RSA modulus.
  name: n
  type: string
- description: RSA public exponent.
  name: e
  type: string
- description: RSA private exponent, or the D component of an EC private key.
  name: d
  type: string
- description: RSA private key parameter.
  name: dp
  type: string
- description: RSA private key parameter.
  name: dq
  type: string
- description: RSA private key parameter.
  name: qi
  type: string
- description: RSA secret prime.
  name: p
  type: string
- description: RSA secret prime, with p < q.
  name: q
  type: string
- description: Symmetric key.
  name: k
  type: string
- description: Protected Key, used with Bring Your Own Key.
  name: key_hsm
  type: string
- description: X component of an EC public key.
  name: x
  type: string
- description: Y component of an EC public key.
  name: y
  type: string
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-json-web-key-schema.json
slug: azure-key-vault-data-plane-json-web-key
source_filename: azure-key-vault-data-plane-json-web-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JsonWebKey\",\n  \"type\": \"object\",\n  \"description\": \"As of http://tools.ietf.org/html/draft-ietf-jose-json-web-key-18.\",\n  \"properties\": {\n    \"kid\": {\n      \"type\": \"string\",\n      \"description\": \"Key identifier.\"\n    },\n    \"key_ops\": {\n      \"type\": \"array\",\n      \"description\": \"Supported key operations.\"\n    },\n    \"n\": {\n      \"type\": \"string\",\n      \"description\": \"RSA modulus.\"\n    },\n    \"e\": {\n      \"type\": \"string\",\n      \"description\": \"RSA public exponent.\"\n    },\n    \"d\": {\n      \"type\": \"string\",\n      \"description\": \"RSA private exponent, or the D component of an EC private key.\"\n    },\n    \"dp\": {\n      \"type\": \"string\",\n      \"description\": \"RSA private key parameter.\"\n    },\n    \"dq\": {\n      \"type\": \"string\",\n      \"description\": \"RSA private key parameter.\"\n    },\n\
  \    \"qi\": {\n      \"type\": \"string\",\n      \"description\": \"RSA private key parameter.\"\n    },\n    \"p\": {\n      \"type\": \"string\",\n      \"description\": \"RSA secret prime.\"\n    },\n    \"q\": {\n      \"type\": \"string\",\n      \"description\": \"RSA secret prime, with p < q.\"\n    },\n    \"k\": {\n      \"type\": \"string\",\n      \"description\": \"Symmetric key.\"\n    },\n    \"key_hsm\": {\n      \"type\": \"string\",\n      \"description\": \"Protected Key, used with Bring Your Own Key.\"\n    },\n    \"x\": {\n      \"type\": \"string\",\n      \"description\": \"X component of an EC public key.\"\n    },\n    \"y\": {\n      \"type\": \"string\",\n      \"description\": \"Y component of an EC public key.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-json-web-key-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: JsonWebKey
---

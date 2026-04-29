---
description: JSON Web Key (JWK) representation of a key.
layout: schema
name: JsonWebKey
properties_list:
- description: Key identifier.
  name: kid
  type: string
- description: Key type (e.g., RSA, EC, oct, oct-HSM).
  name: kty
  type: string
- description: Allowed key operations.
  name: key_ops
  type: array
- description: RSA modulus.
  name: n
  type: string
- description: RSA public exponent.
  name: e
  type: string
- description: RSA private exponent.
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
- description: RSA secret prime.
  name: q
  type: string
- description: Symmetric key.
  name: k
  type: string
- description: Elliptic curve name.
  name: crv
  type: string
- description: X component of an EC public key.
  name: x
  type: string
- description: Y component of an EC public key.
  name: y
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-json-web-key-schema.json
slug: azure-key-vault-json-web-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JsonWebKey\",\n  \"type\": \"object\",\n  \"description\": \"JSON Web Key (JWK) representation of a key.\",\n  \"properties\": {\n    \"kid\": {\n      \"type\": \"string\",\n      \"description\": \"Key identifier.\"\n    },\n    \"kty\": {\n      \"type\": \"string\",\n      \"description\": \"Key type (e.g., RSA, EC, oct, oct-HSM).\"\n    },\n    \"key_ops\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed key operations.\"\n    },\n    \"n\": {\n      \"type\": \"string\",\n      \"description\": \"RSA modulus.\"\n    },\n    \"e\": {\n      \"type\": \"string\",\n      \"description\": \"RSA public exponent.\"\n    },\n    \"d\": {\n      \"type\": \"string\",\n      \"description\": \"RSA private exponent.\"\n    },\n    \"dp\": {\n      \"type\": \"string\",\n      \"description\": \"RSA private key parameter.\"\n    },\n    \"dq\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"RSA private key parameter.\"\n    },\n    \"qi\": {\n      \"type\": \"string\",\n      \"description\": \"RSA private key parameter.\"\n    },\n    \"p\": {\n      \"type\": \"string\",\n      \"description\": \"RSA secret prime.\"\n    },\n    \"q\": {\n      \"type\": \"string\",\n      \"description\": \"RSA secret prime.\"\n    },\n    \"k\": {\n      \"type\": \"string\",\n      \"description\": \"Symmetric key.\"\n    },\n    \"crv\": {\n      \"type\": \"string\",\n      \"description\": \"Elliptic curve name.\"\n    },\n    \"x\": {\n      \"type\": \"string\",\n      \"description\": \"X component of an EC public key.\"\n    },\n    \"y\": {\n      \"type\": \"string\",\n      \"description\": \"Y component of an EC public key.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-json-web-key-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: JsonWebKey
---

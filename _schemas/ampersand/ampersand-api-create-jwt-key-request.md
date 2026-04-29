---
description: CreateJWTKeyRequest schema from Ampersand API
layout: schema
name: CreateJWTKeyRequest
properties_list:
- description: Human-readable label for the JWT key
  name: label
  type: string
- description: The cryptographic JWT signing algorithm (currently only RS256 is supported)
  name: algorithm
  type: string
- description: RSA public key in PEM format for JWT signature verification
  name: publicKeyPem
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-create-jwt-key-request-schema.json
slug: ampersand-api-create-jwt-key-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-create-jwt-key-request-schema.json\",\n  \"title\": \"CreateJWTKeyRequest\",\n  \"description\": \"CreateJWTKeyRequest schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable label for the JWT key\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"example\": \"production-key-1\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"description\": \"The cryptographic JWT signing algorithm (currently only RS256 is supported)\",\n      \"enum\": [\n        \"RS256\"\n      ],\n      \"example\": \"RS256\"\n    },\n    \"publicKeyPem\": {\n      \"type\": \"string\",\n      \"description\": \"RSA public key in PEM format for JWT signature verification\",\n      \"format\"\
  : \"pem\",\n      \"example\": \"-----BEGIN PUBLIC KEY-----\\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA4f5wg5l2hKsTeNem/V41\\nfGnJm6gOdrj8ym3rFkEjWT2btf2QisEgQG5WQwTfEUvUNR8JW5FQ0mKJ5I4LhXq6\\nV5gN6kSKs2cUdD8Ky7Lj7kqn6I3l3r3F2fK9MFjZ8tU5z4z4yHdF6W2C3k5vf3f\\n-----END PUBLIC KEY-----\\n\"\n    }\n  },\n  \"required\": [\n    \"label\",\n    \"algorithm\",\n    \"publicKeyPem\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-create-jwt-key-request-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: CreateJWTKeyRequest
---

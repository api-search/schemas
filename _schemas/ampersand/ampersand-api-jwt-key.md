---
description: JWTKey schema from Ampersand API
layout: schema
name: JWTKey
properties_list:
- description: Unique identifier for the JWT key
  name: id
  type: string
- description: The project this JWT key belongs to
  name: projectId
  type: string
- description: Human-readable name for the JWT key
  name: label
  type: string
- description: The cryptographic algorithm used
  name: algorithm
  type: string
- description: RSA public key in PEM format
  name: publicKeyPem
  type: string
- description: Whether the JWT key is currently active and can be used for verification
  name: active
  type: boolean
- description: Timestamp when the JWT key was created
  name: createTime
  type: string
- description: Timestamp when the JWT key was last updated
  name: updateTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-jwt-key-schema.json
slug: ampersand-api-jwt-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-jwt-key-schema.json\",\n  \"title\": \"JWTKey\",\n  \"description\": \"JWTKey schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the JWT key\",\n      \"example\": \"550e8400-e29b-41d4-a716-446655440000\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The project this JWT key belongs to\",\n      \"example\": \"123e4567-e89b-12d3-a456-426614174000\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the JWT key\",\n      \"example\": \"production-key-1\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The cryptographic algorithm used\",\n      \"enum\": [\n        \"RSA\"\n      ],\n      \"example\": \"RSA\"\n    },\n    \"publicKeyPem\": {\n      \"type\": \"string\",\n      \"description\": \"RSA public key in PEM format\",\n      \"format\": \"pem\",\n      \"example\": \"-----BEGIN PUBLIC KEY-----\\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA4f5wg5l2hKsTeNem/V41\\n-----END PUBLIC KEY-----\\n\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the JWT key is currently active and can be used for verification\",\n      \"example\": true\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the JWT key was created\",\n      \"example\": \"2024-01-15T10:30:00Z\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the JWT key was last updated\",\n      \"example\": \"2024-01-15T10:30:00Z\"\
  \n    }\n  },\n  \"required\": [\n    \"id\",\n    \"projectId\",\n    \"label\",\n    \"algorithm\",\n    \"publicKeyPem\",\n    \"active\",\n    \"createTime\",\n    \"updateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-jwt-key-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: JWTKey
---

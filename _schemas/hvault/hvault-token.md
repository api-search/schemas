---
description: Represents an authentication token in HashiCorp Vault used to authenticate API requests and carry identity and policy information.
layout: schema
name: Vault Token
properties_list:
- description: Token accessor used for token management without exposing the token ID
  name: accessor
  type: string
- description: Token creation time as Unix epoch seconds
  name: creation_time
  type: integer
- description: Original TTL in seconds
  name: creation_ttl
  type: integer
- description: Human-readable display name for the token
  name: display_name
  type: string
- description: Identity entity ID associated with the token
  name: entity_id
  type: string
- description: Token expiration time
  name: expire_time
  type: string
- description: Explicit maximum TTL in seconds
  name: explicit_max_ttl
  type: integer
- description: Token ID (the actual secret value)
  name: id
  type: string
- description: Token issue time
  name: issue_time
  type: string
- description: Metadata key-value pairs associated with the token
  name: meta
  type: object
- description: Remaining number of uses (0 for unlimited)
  name: num_uses
  type: integer
- description: Whether the token is an orphan (no parent token)
  name: orphan
  type: boolean
- description: Auth path that created this token
  name: path
  type: string
- description: Policies attached to the token
  name: policies
  type: array
- description: Whether the token is renewable
  name: renewable
  type: boolean
- description: Remaining TTL in seconds
  name: ttl
  type: integer
- description: Token type
  name: type
  type: string
provider_name: HashiCorp Vault
provider_slug: hvault
schema_file: json-schema/hvault-token-schema.json
slug: hvault-token
source_filename: hvault-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.hashicorp.com/schemas/vault/token.json\",\n  \"title\": \"Vault Token\",\n  \"description\": \"Represents an authentication token in HashiCorp Vault used to authenticate API requests and carry identity and policy information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessor\": {\n      \"type\": \"string\",\n      \"description\": \"Token accessor used for token management without exposing the token ID\"\n    },\n    \"creation_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Token creation time as Unix epoch seconds\"\n    },\n    \"creation_ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Original TTL in seconds\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the token\"\n    },\n    \"entity_id\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"Identity entity ID associated with the token\"\n    },\n    \"expire_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Token expiration time\"\n    },\n    \"explicit_max_ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Explicit maximum TTL in seconds\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Token ID (the actual secret value)\"\n    },\n    \"issue_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Token issue time\"\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Metadata key-value pairs associated with the token\"\n    },\n    \"num_uses\": {\n      \"type\": \"integer\",\n      \"description\": \"Remaining number of uses (0 for unlimited)\"\n    },\n    \"orphan\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the token is an orphan (no parent token)\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Auth path that created this token\"\n    },\n    \"policies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Policies attached to the token\"\n    },\n    \"renewable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the token is renewable\"\n    },\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Remaining TTL in seconds\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"service\", \"batch\"],\n      \"description\": \"Token type\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/json-schema/hvault-token-schema.json
tags:
- Encryption
- Identity
- Infrastructure
- Secrets Management
- Security
title: Vault Token
---

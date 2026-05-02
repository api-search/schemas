---
description: Represents an entity alias that maps an authentication method identity to a Vault identity entity.
layout: schema
name: Vault Entity Alias
properties_list:
- description: Unique identifier for the alias
  name: id
  type: string
- description: Entity ID this alias belongs to
  name: canonical_id
  type: string
- description: Auth mount accessor that created this alias
  name: mount_accessor
  type: string
- description: Auth mount path
  name: mount_path
  type: string
- description: Auth mount type (e.g., token, approle, ldap)
  name: mount_type
  type: string
- description: Name of the alias within the auth method
  name: name
  type: string
- description: Metadata from the auth method
  name: metadata
  type: object
- description: Alias creation timestamp
  name: creation_time
  type: string
- description: Last update timestamp
  name: last_update_time
  type: string
provider_name: HashiCorp Vault
provider_slug: hvault
schema_file: json-schema/hvault-entity-alias-schema.json
slug: hvault-entity-alias
source_filename: hvault-entity-alias-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.hashicorp.com/schemas/vault/entity-alias.json\",\n  \"title\": \"Vault Entity Alias\",\n  \"description\": \"Represents an entity alias that maps an authentication method identity to a Vault identity entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the alias\"\n    },\n    \"canonical_id\": {\n      \"type\": \"string\",\n      \"description\": \"Entity ID this alias belongs to\"\n    },\n    \"mount_accessor\": {\n      \"type\": \"string\",\n      \"description\": \"Auth mount accessor that created this alias\"\n    },\n    \"mount_path\": {\n      \"type\": \"string\",\n      \"description\": \"Auth mount path\"\n    },\n    \"mount_type\": {\n      \"type\": \"string\",\n      \"description\": \"Auth mount type (e.g., token, approle, ldap)\"\n    },\n    \"name\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Name of the alias within the auth method\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Metadata from the auth method\"\n    },\n    \"creation_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Alias creation timestamp\"\n    },\n    \"last_update_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/json-schema/hvault-entity-alias-schema.json
tags:
- Encryption
- Identity
- Infrastructure
- Secrets Management
- Security
title: Vault Entity Alias
---

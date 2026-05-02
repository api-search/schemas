---
description: Represents a versioned secret stored in the Vault KV v2 secrets engine, including its data payload and version metadata.
layout: schema
name: Vault Secret
properties_list:
- description: The secret key-value data
  name: data
  type: object
- description: Version metadata for the secret
  name: metadata
  type: object
provider_name: HashiCorp Vault
provider_slug: hvault
schema_file: json-schema/hvault-secret-schema.json
slug: hvault-secret
source_filename: hvault-secret-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.hashicorp.com/schemas/vault/secret.json\",\n  \"title\": \"Vault Secret\",\n  \"description\": \"Represents a versioned secret stored in the Vault KV v2 secrets engine, including its data payload and version metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"The secret key-value data\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"created_time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When this version was created\"\n        },\n        \"custom_metadata\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Custom metadata key-value pairs\"\n       \
  \ },\n        \"deletion_time\": {\n          \"type\": \"string\",\n          \"description\": \"When this version was deleted (empty if not deleted)\"\n        },\n        \"destroyed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version has been permanently destroyed\"\n        },\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"Version number\"\n        }\n      },\n      \"description\": \"Version metadata for the secret\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/json-schema/hvault-secret-schema.json
tags:
- Encryption
- Identity
- Infrastructure
- Secrets Management
- Security
title: Vault Secret
---

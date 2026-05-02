---
description: Represents an identity entity in HashiCorp Vault that provides a unified view of a user or machine across multiple authentication methods.
layout: schema
name: Vault Identity Entity
properties_list:
- description: Unique identifier for the entity
  name: id
  type: string
- description: Name of the entity
  name: name
  type: string
- description: Metadata key-value pairs associated with the entity
  name: metadata
  type: object
- description: Whether the entity is disabled
  name: disabled
  type: boolean
- description: Authentication method aliases for this entity
  name: aliases
  type: array
- description: IDs of groups the entity directly belongs to
  name: direct_group_ids
  type: array
- description: IDs of groups inherited through group hierarchy
  name: inherited_group_ids
  type: array
- description: Policies directly assigned to the entity
  name: policies
  type: array
- description: Entity creation timestamp
  name: creation_time
  type: string
- description: Last update timestamp
  name: last_update_time
  type: string
provider_name: HashiCorp Vault
provider_slug: hvault
schema_file: json-schema/hvault-entity-schema.json
slug: hvault-entity
source_filename: hvault-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.hashicorp.com/schemas/vault/entity.json\",\n  \"title\": \"Vault Identity Entity\",\n  \"description\": \"Represents an identity entity in HashiCorp Vault that provides a unified view of a user or machine across multiple authentication methods.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the entity\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the entity\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Metadata key-value pairs associated with the entity\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the entity is disabled\"\n    },\n    \"aliases\": {\n      \"type\": \"array\",\n\
  \      \"items\": {\n        \"$ref\": \"hvault-entity-alias-schema.json\"\n      },\n      \"description\": \"Authentication method aliases for this entity\"\n    },\n    \"direct_group_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of groups the entity directly belongs to\"\n    },\n    \"inherited_group_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of groups inherited through group hierarchy\"\n    },\n    \"policies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Policies directly assigned to the entity\"\n    },\n    \"creation_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Entity creation timestamp\"\n    },\n    \"last_update_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n\
  \      \"description\": \"Last update timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/json-schema/hvault-entity-schema.json
tags:
- Encryption
- Identity
- Infrastructure
- Secrets Management
- Security
title: Vault Identity Entity
---

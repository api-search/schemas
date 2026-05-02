---
description: Represents an identity group in HashiCorp Vault that organizes entities and provides group-level policy assignment.
layout: schema
name: Vault Identity Group
properties_list:
- description: Unique identifier for the group
  name: id
  type: string
- description: Name of the group
  name: name
  type: string
- description: Group type (internal for manual membership, external for auth-method-based)
  name: type
  type: string
- description: Metadata key-value pairs
  name: metadata
  type: object
- description: Policies assigned to the group
  name: policies
  type: array
- description: Entity IDs that are members of this group
  name: member_entity_ids
  type: array
- description: Group IDs that are subgroups of this group
  name: member_group_ids
  type: array
- description: Parent group IDs
  name: parent_group_ids
  type: array
- description: Group creation timestamp
  name: creation_time
  type: string
- description: Last update timestamp
  name: last_update_time
  type: string
provider_name: HashiCorp Vault
provider_slug: hvault
schema_file: json-schema/hvault-group-schema.json
slug: hvault-group
source_filename: hvault-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.hashicorp.com/schemas/vault/group.json\",\n  \"title\": \"Vault Identity Group\",\n  \"description\": \"Represents an identity group in HashiCorp Vault that organizes entities and provides group-level policy assignment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the group\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the group\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"internal\", \"external\"],\n      \"description\": \"Group type (internal for manual membership, external for auth-method-based)\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Metadata key-value pairs\"\n    },\n    \"policies\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Policies assigned to the group\"\n    },\n    \"member_entity_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Entity IDs that are members of this group\"\n    },\n    \"member_group_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Group IDs that are subgroups of this group\"\n    },\n    \"parent_group_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Parent group IDs\"\n    },\n    \"creation_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Group creation timestamp\"\n    },\n    \"last_update_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update\
  \ timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/json-schema/hvault-group-schema.json
tags:
- Encryption
- Identity
- Infrastructure
- Secrets Management
- Security
title: Vault Identity Group
---

---
description: A managed role object in the ForgeRock Identity Platform. Roles define collections of privileges and can be assigned to users either directly or through conditional membership rules.
layout: schema
name: ForgeRock Managed Role
properties_list:
- description: Unique identifier assigned by the system
  name: _id
  type: string
- description: Object revision string for optimistic concurrency control
  name: _rev
  type: string
- description: Role name
  name: name
  type: string
- description: Role description
  name: description
  type: string
- description: Query filter expression for conditional (dynamic) role membership. Users matching this condition are automatically assigned the role.
  name: condition
  type: string
- description: Time-based constraints for role activation. The role is only active during the specified time windows.
  name: temporalConstraints
  type: array
- description: References to assignment objects that define what this role grants on connected systems
  name: assignments
  type: array
- description: References to user objects that are members of this role
  name: members
  type: array
provider_name: ForgeRock
provider_slug: forgerock
schema_file: json-schema/forgerock-managed-role-schema.json
slug: forgerock-managed-role
source_filename: forgerock-managed-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.forgerock.com/managed-role\",\n  \"title\": \"ForgeRock Managed Role\",\n  \"description\": \"A managed role object in the ForgeRock Identity Platform. Roles define collections of privileges and can be assigned to users either directly or through conditional membership rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by the system\",\n      \"readOnly\": true\n    },\n    \"_rev\": {\n      \"type\": \"string\",\n      \"description\": \"Object revision string for optimistic concurrency control\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Role name\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Role description\"\n    },\n    \"condition\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"Query filter expression for conditional (dynamic) role membership. Users matching this condition are automatically assigned the role.\"\n    },\n    \"temporalConstraints\": {\n      \"type\": \"array\",\n      \"description\": \"Time-based constraints for role activation. The role is only active during the specified time windows.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"duration\": {\n            \"type\": \"string\",\n            \"description\": \"ISO 8601 time interval (e.g., 2024-01-01T00:00:00Z/2024-12-31T23:59:59Z)\"\n          }\n        },\n        \"required\": [\"duration\"]\n      }\n    },\n    \"assignments\": {\n      \"type\": \"array\",\n      \"description\": \"References to assignment objects that define what this role grants on connected systems\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"_ref\": {\n            \"\
  type\": \"string\",\n            \"description\": \"Reference path to the assignment object\"\n          },\n          \"_refProperties\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"References to user objects that are members of this role\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"_ref\": {\n            \"type\": \"string\"\n          },\n          \"_refProperties\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"name\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/json-schema/forgerock-managed-role-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity Governance
- Identity Management
- OAuth
- OpenID Connect
title: ForgeRock Managed Role
---

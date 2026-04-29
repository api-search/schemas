---
description: Role schema from Palo Alto Networks SASE IAM Service API
layout: schema
name: Role
properties_list:
- description: Unique identifier of the role.
  name: id
  type: string
- description: Role name (e.g., superuser, network_admin, readonly).
  name: name
  type: string
- description: Human-readable role display name.
  name: display_name
  type: string
- description: Description of the permissions granted by this role.
  name: description
  type: string
- description: List of permission identifiers included in this role.
  name: permissions
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-iam-api-role-schema.json
slug: sase-iam-api-role
source_filename: sase-iam-api-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Role\",\n  \"description\": \"Role schema from Palo Alto Networks SASE IAM Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-role-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the role.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Role name (e.g., superuser, network_admin, readonly).\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable role display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the permissions granted by this role.\"\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n\
  \      \"description\": \"List of permission identifiers included in this role.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-role-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Role
---

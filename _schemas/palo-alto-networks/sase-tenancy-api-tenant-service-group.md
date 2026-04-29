---
description: TenantServiceGroup schema from Palo Alto Networks SASE Tenancy Service API
layout: schema
name: TenantServiceGroup
properties_list:
- description: Unique identifier of the Tenant Service Group.
  name: id
  type: string
- description: Human-readable display name of the TSG.
  name: display_name
  type: string
- description: Optional description of the TSG's purpose.
  name: description
  type: string
- description: ID of the parent TSG in the hierarchy. Null for root-level TSGs.
  name: parent_id
  type: string
- description: Associated Palo Alto Networks support account identifier.
  name: support_account_id
  type: string
- description: Industry vertical classification for the TSG.
  name: vertical
  type: string
- description: Primary geographic region for the TSG.
  name: region
  type: string
- description: Current status of the TSG.
  name: status
  type: string
- description: Number of direct child TSGs.
  name: child_count
  type: integer
- description: Timestamp when the TSG was created.
  name: created_at
  type: string
- description: Timestamp of the most recent TSG modification.
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-tenancy-api-tenant-service-group-schema.json
slug: sase-tenancy-api-tenant-service-group
source_filename: sase-tenancy-api-tenant-service-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantServiceGroup\",\n  \"description\": \"TenantServiceGroup schema from Palo Alto Networks SASE Tenancy Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-tenancy-api-tenant-service-group-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the Tenant Service Group.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name of the TSG.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the TSG's purpose.\"\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent TSG in the hierarchy. Null for root-level TSGs.\"\n    },\n    \"support_account_id\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Associated Palo Alto Networks support account identifier.\"\n    },\n    \"vertical\": {\n      \"type\": \"string\",\n      \"description\": \"Industry vertical classification for the TSG.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Primary geographic region for the TSG.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"suspended\",\n        \"pending\"\n      ],\n      \"description\": \"Current status of the TSG.\"\n    },\n    \"child_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of direct child TSGs.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the TSG was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent\
  \ TSG modification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-tenancy-api-tenant-service-group-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantServiceGroup
---

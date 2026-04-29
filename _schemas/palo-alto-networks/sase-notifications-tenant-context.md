---
description: Tenant context information for multitenant notification routing.
layout: schema
name: TenantContext
properties_list:
- description: Tenant Service Group identifier.
  name: tsg_id
  type: string
- description: Human-readable tenant name.
  name: tenantName
  type: string
- description: Parent Tenant Service Group identifier for hierarchical tenant structures.
  name: parentTsgId
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-notifications-tenant-context-schema.json
slug: sase-notifications-tenant-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantContext\",\n  \"description\": \"Tenant context information for multitenant notification routing.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-tenant-context-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service Group identifier.\"\n    },\n    \"tenantName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable tenant name.\"\n    },\n    \"parentTsgId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent Tenant Service Group identifier for hierarchical tenant structures.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-tenant-context-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantContext
---

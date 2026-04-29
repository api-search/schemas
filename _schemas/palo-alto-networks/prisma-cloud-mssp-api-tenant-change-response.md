---
description: 'TenantChangeResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: TenantChangeResponse
properties_list:
- description: ''
  name: tenantChangeId
  type: string
- description: ''
  name: externalTenantId
  type: string
- description: ''
  name: tenantPrismaId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: updatedAt
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-tenant-change-response-schema.json
slug: prisma-cloud-mssp-api-tenant-change-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantChangeResponse\",\n  \"description\": \"TenantChangeResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-change-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tenantChangeId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"externalTenantId\": {\n      \"type\": \"string\"\n    },\n    \"tenantPrismaId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IN_PROGRESS\",\n        \"SUCCESS\",\n        \"FAILURE\"\n      ]\n    },\n    \"updatedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-change-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantChangeResponse
---

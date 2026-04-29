---
description: 'TenantGroupResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: TenantGroupResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: groupName
  type: string
- description: ''
  name: tenants
  type: array
- description: ''
  name: createdAt
  type: integer
- description: ''
  name: createdBy
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-tenant-group-response-schema.json
slug: prisma-cloud-mssp-api-tenant-group-response
source_filename: prisma-cloud-mssp-api-tenant-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantGroupResponse\",\n  \"description\": \"TenantGroupResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"groupName\": {\n      \"type\": \"string\"\n    },\n    \"tenants\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"externalTenantId\": {\n            \"type\": \"string\"\n          },\n          \"prismaId\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"createdBy\"\
  : {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantGroupResponse
---

---
description: 'TenantGroupMappingDetails schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: TenantGroupMappingDetails
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: tenantGroupId
  type: string
- description: ''
  name: tenantGroupName
  type: string
- description: ''
  name: tenantCount
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-tenant-group-mapping-details-schema.json
slug: prisma-cloud-mssp-api-tenant-group-mapping-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantGroupMappingDetails\",\n  \"description\": \"TenantGroupMappingDetails schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-mapping-details-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"tenantGroupId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"tenantGroupName\": {\n      \"type\": \"string\"\n    },\n    \"tenantCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-mapping-details-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantGroupMappingDetails
---

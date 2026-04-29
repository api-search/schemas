---
description: 'CreateTenantGroupRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: CreateTenantGroupRequest
properties_list:
- description: ''
  name: groupName
  type: string
- description: ''
  name: tenantIds
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-create-tenant-group-request-schema.json
slug: prisma-cloud-mssp-api-create-tenant-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTenantGroupRequest\",\n  \"description\": \"CreateTenantGroupRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-create-tenant-group-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupName\": {\n      \"maxLength\": 63,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"tenantIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"groupName\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-create-tenant-group-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CreateTenantGroupRequest
---

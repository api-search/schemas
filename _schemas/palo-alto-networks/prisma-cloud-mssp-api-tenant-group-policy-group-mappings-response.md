---
description: 'TenantGroupPolicyGroupMappingsResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: TenantGroupPolicyGroupMappingsResponse
properties_list:
- description: ''
  name: value
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-tenant-group-policy-group-mappings-response-schema.json
slug: prisma-cloud-mssp-api-tenant-group-policy-group-mappings-response
source_filename: prisma-cloud-mssp-api-tenant-group-policy-group-mappings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantGroupPolicyGroupMappingsResponse\",\n  \"description\": \"TenantGroupPolicyGroupMappingsResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-policy-group-mappings-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"tenantGroupId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"policyGroupId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-policy-group-mappings-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantGroupPolicyGroupMappingsResponse
---

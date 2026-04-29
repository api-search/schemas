---
description: 'TenantGroupPolicyGroupMapRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: TenantGroupPolicyGroupMapRequest
properties_list:
- description: Tenant group to Policy groups mappings.
  name: mappings
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-tenant-group-policy-group-map-request-schema.json
slug: prisma-cloud-mssp-api-tenant-group-policy-group-map-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantGroupPolicyGroupMapRequest\",\n  \"description\": \"TenantGroupPolicyGroupMapRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-policy-group-map-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mappings\": {\n      \"type\": \"array\",\n      \"description\": \"Tenant group to Policy groups mappings.\",\n      \"items\": {\n        \"required\": [\n          \"policyGroupIds\",\n          \"tenantGroupId\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"tenantGroupId\": {\n            \"type\": \"string\",\n            \"description\": \"Tenant group to which the policy groups are mapped.\",\n            \"format\": \"uuid\"\n          },\n          \"policyGroupIds\"\
  : {\n            \"type\": \"array\",\n            \"description\": \"Policy groups to be mapped.\",\n            \"items\": {\n              \"type\": \"string\",\n              \"description\": \"Policy groups to be mapped.\",\n              \"format\": \"uuid\"\n            }\n          }\n        },\n        \"description\": \"Tenant group to Policy groups mappings.\"\n      }\n    }\n  },\n  \"required\": [\n    \"mappings\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-policy-group-map-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantGroupPolicyGroupMapRequest
---

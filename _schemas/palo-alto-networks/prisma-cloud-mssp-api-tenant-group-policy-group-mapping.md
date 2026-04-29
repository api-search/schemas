---
description: Tenant group to Policy groups mappings.
layout: schema
name: TenantGroupPolicyGroupMapping
properties_list:
- description: Tenant group to which the policy groups are mapped.
  name: tenantGroupId
  type: string
- description: Policy groups to be mapped.
  name: policyGroupIds
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-tenant-group-policy-group-mapping-schema.json
slug: prisma-cloud-mssp-api-tenant-group-policy-group-mapping
source_filename: prisma-cloud-mssp-api-tenant-group-policy-group-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TenantGroupPolicyGroupMapping\",\n  \"description\": \"Tenant group to Policy groups mappings.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-policy-group-mapping-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tenantGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant group to which the policy groups are mapped.\",\n      \"format\": \"uuid\"\n    },\n    \"policyGroupIds\": {\n      \"type\": \"array\",\n      \"description\": \"Policy groups to be mapped.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Policy groups to be mapped.\",\n        \"format\": \"uuid\"\n      }\n    }\n  },\n  \"required\": [\n    \"policyGroupIds\",\n    \"tenantGroupId\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-tenant-group-policy-group-mapping-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TenantGroupPolicyGroupMapping
---

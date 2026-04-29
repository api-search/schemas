---
description: 'UpdateManagedTenantRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: UpdateManagedTenantRequest
properties_list:
- description: ''
  name: tenantGroupId
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: licenseInfo
  type: object
- description: ''
  name: modules
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-update-managed-tenant-request-schema.json
slug: prisma-cloud-mssp-api-update-managed-tenant-request
source_filename: prisma-cloud-mssp-api-update-managed-tenant-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateManagedTenantRequest\",\n  \"description\": \"UpdateManagedTenantRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-update-managed-tenant-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tenantGroupId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"companyName\": {\n      \"maxLength\": 63,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"licenseInfo\": {\n      \"required\": [\n        \"allocatedCredits\",\n        \"licensePoolId\"\n      ],\n      \"type\": \"object\",\n      \"properties\": {\n        \"licensePoolId\": {\n          \"type\": \"string\"\n        },\n        \"allocatedCredits\": {\n          \"minimum\": 1,\n          \"type\": \"integer\"\
  ,\n          \"format\": \"int32\"\n        }\n      }\n    },\n    \"modules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"required\": [\n          \"enabled\",\n          \"featureName\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"featureName\": {\n            \"pattern\": \"iam-security\",\n            \"type\": \"string\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\"\n          },\n          \"additionalData\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-update-managed-tenant-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: UpdateManagedTenantRequest
---

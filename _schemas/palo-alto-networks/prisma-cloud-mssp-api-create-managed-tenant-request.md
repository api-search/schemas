---
description: 'CreateManagedTenantRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: CreateManagedTenantRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: tenantGroupId
  type: string
- description: ''
  name: planType
  type: string
- description: ''
  name: contactInfo
  type: object
- description: ''
  name: licenseInfo
  type: object
- description: ''
  name: modules
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-create-managed-tenant-request-schema.json
slug: prisma-cloud-mssp-api-create-managed-tenant-request
source_filename: prisma-cloud-mssp-api-create-managed-tenant-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateManagedTenantRequest\",\n  \"description\": \"CreateManagedTenantRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-create-managed-tenant-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"maxLength\": 63,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"maxLength\": 63,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"tenantGroupId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"planType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RS_STANDARD\",\n        \"RS_FOUNDATION\",\n        \"RS_ADVANCED\"\n      ]\n    },\n    \"\
  contactInfo\": {\n      \"required\": [\n        \"email\",\n        \"firstName\",\n        \"lastName\"\n      ],\n      \"type\": \"object\",\n      \"properties\": {\n        \"firstName\": {\n          \"maxLength\": 63,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        },\n        \"lastName\": {\n          \"maxLength\": 63,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        },\n        \"email\": {\n          \"maxLength\": 128,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"licenseInfo\": {\n      \"required\": [\n        \"allocatedCredits\",\n        \"licensePoolId\"\n      ],\n      \"type\": \"object\",\n      \"properties\": {\n        \"licensePoolId\": {\n          \"type\": \"string\"\n        },\n        \"allocatedCredits\": {\n          \"minimum\": 1,\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        }\n      }\n    },\n    \"modules\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"required\": [\n          \"enabled\",\n          \"featureName\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"featureName\": {\n            \"pattern\": \"iam-security\",\n            \"type\": \"string\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\"\n          },\n          \"additionalData\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"companyName\",\n    \"contactInfo\",\n    \"licenseInfo\",\n    \"name\",\n    \"planType\",\n    \"region\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-create-managed-tenant-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CreateManagedTenantRequest
---

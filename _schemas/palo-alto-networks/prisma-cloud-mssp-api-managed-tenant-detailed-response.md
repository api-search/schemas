---
description: 'ManagedTenantDetailedResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: ManagedTenantDetailedResponse
properties_list:
- description: ''
  name: prismaId
  type: string
- description: ''
  name: externalTenantId
  type: string
- description: ''
  name: customerName
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: isSynthetic
  type: boolean
- description: ''
  name: wasMigrated
  type: boolean
- description: ''
  name: msspId
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
  name: stack
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: baseApiUrl
  type: string
- description: ''
  name: tenantLicense
  type: object
- description: ''
  name: createdBy
  type: string
- description: ''
  name: createdAt
  type: integer
- description: ''
  name: modules
  type: array
- description: ''
  name: erroredBy
  type: string
- description: ''
  name: policyGroups
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-managed-tenant-detailed-response-schema.json
slug: prisma-cloud-mssp-api-managed-tenant-detailed-response
source_filename: prisma-cloud-mssp-api-managed-tenant-detailed-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedTenantDetailedResponse\",\n  \"description\": \"ManagedTenantDetailedResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-managed-tenant-detailed-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prismaId\": {\n      \"type\": \"string\"\n    },\n    \"externalTenantId\": {\n      \"type\": \"string\"\n    },\n    \"customerName\": {\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"PROVISIONING\",\n        \"UPDATING\",\n        \"DELETING\",\n        \"DELETED\",\n        \"OFFBOARDING\",\n        \"ERRORED\"\n      ]\n    },\n    \"isSynthetic\": {\n      \"\
  type\": \"boolean\"\n    },\n    \"wasMigrated\": {\n      \"type\": \"boolean\"\n    },\n    \"msspId\": {\n      \"type\": \"string\"\n    },\n    \"tenantGroupId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"planType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RS_STANDARD\",\n        \"RS_FOUNDATION\",\n        \"RS_ADVANCED\"\n      ]\n    },\n    \"contactInfo\": {\n      \"required\": [\n        \"email\",\n        \"firstName\",\n        \"lastName\"\n      ],\n      \"type\": \"object\",\n      \"properties\": {\n        \"firstName\": {\n          \"maxLength\": 63,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        },\n        \"lastName\": {\n          \"maxLength\": 63,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        },\n        \"email\": {\n          \"maxLength\": 128,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"stack\": {\n    \
  \  \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"baseApiUrl\": {\n      \"type\": \"string\"\n    },\n    \"tenantLicense\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"tenantLicenseId\": {\n          \"type\": \"string\"\n        },\n        \"serialNumber\": {\n          \"type\": \"string\"\n        },\n        \"licensePoolId\": {\n          \"type\": \"string\"\n        },\n        \"allocatedCredits\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        },\n        \"startDate\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"endDate\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        }\n      }\n    },\n    \"createdBy\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"modules\": {\n      \"type\": \"array\",\n      \"items\": {\n\
  \        \"required\": [\n          \"feature_name\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"feature_name\": {\n            \"type\": \"string\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\"\n          },\n          \"billing_type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"TRIAL\",\n              \"BUY\"\n            ]\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"PROVISION_STARTED\",\n              \"PROVISION_SUCCESSFUL\",\n              \"PROVISION_FAILED\"\n            ]\n          },\n          \"additional_data\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    },\n    \"erroredBy\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"policyGroups\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"policyCount\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-managed-tenant-detailed-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ManagedTenantDetailedResponse
---

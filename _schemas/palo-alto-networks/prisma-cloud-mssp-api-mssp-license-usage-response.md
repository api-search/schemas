---
description: 'MsspLicenseUsageResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: MsspLicenseUsageResponse
properties_list:
- description: ''
  name: value
  type: array
- description: ''
  name: nextPageToken
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-mssp-license-usage-response-schema.json
slug: prisma-cloud-mssp-api-mssp-license-usage-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MsspLicenseUsageResponse\",\n  \"description\": \"MsspLicenseUsageResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-usage-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"tenantName\": {\n            \"type\": \"string\"\n          },\n          \"prismaId\": {\n            \"type\": \"string\"\n          },\n          \"createdOn\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"expiringOn\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"status\": {\n        \
  \    \"type\": \"string\",\n            \"enum\": [\n              \"ACTIVE\",\n              \"PROVISIONING\",\n              \"UPDATING\",\n              \"DELETING\",\n              \"DELETED\",\n              \"OFFBOARDING\",\n              \"ERRORED\"\n            ]\n          },\n          \"creditsAllocated\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          },\n          \"avgConsumption\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          },\n          \"lastUpdated\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"externalTenantId\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-usage-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MsspLicenseUsageResponse
---

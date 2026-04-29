---
description: 'MsspLicensePoolsResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: MsspLicensePoolsResponse
properties_list:
- description: ''
  name: value
  type: array
- description: ''
  name: nextPageToken
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-mssp-license-pools-response-schema.json
slug: prisma-cloud-mssp-api-mssp-license-pools-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MsspLicensePoolsResponse\",\n  \"description\": \"MsspLicensePoolsResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-pools-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"licensePoolId\": {\n            \"type\": \"string\"\n          },\n          \"poolName\": {\n            \"type\": \"string\"\n          },\n          \"serialNumber\": {\n            \"type\": \"string\"\n          },\n          \"msspId\": {\n            \"type\": \"string\"\n          },\n          \"totalCredits\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n   \
  \       },\n          \"unallocatedCredits\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          },\n          \"startDate\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"endDate\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"tenantLicenses\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"tenantLicenseId\": {\n                  \"type\": \"string\"\n                },\n                \"serialNumber\": {\n                  \"type\": \"string\"\n                },\n                \"licensePoolId\": {\n                  \"type\": \"string\"\n                },\n                \"allocatedCredits\": {\n                  \"type\": \"integer\",\n                  \"format\": \"int32\"\n                },\n                \"startDate\": {\n     \
  \             \"type\": \"integer\",\n                  \"format\": \"int64\"\n                },\n                \"endDate\": {\n                  \"type\": \"integer\",\n                  \"format\": \"int64\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-pools-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MsspLicensePoolsResponse
---

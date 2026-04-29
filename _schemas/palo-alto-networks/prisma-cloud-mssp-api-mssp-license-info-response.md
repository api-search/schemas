---
description: 'MsspLicenseInfoResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: MsspLicenseInfoResponse
properties_list:
- description: ''
  name: creditsPurchased
  type: integer
- description: ''
  name: creditsAllocated
  type: integer
- description: ''
  name: balanceCredit
  type: integer
- description: ''
  name: numOfTenant
  type: integer
- description: ''
  name: startTime
  type: integer
- description: ''
  name: endTime
  type: integer
- description: ''
  name: msspLicensePoolInfos
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-mssp-license-info-response-schema.json
slug: prisma-cloud-mssp-api-mssp-license-info-response
source_filename: prisma-cloud-mssp-api-mssp-license-info-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MsspLicenseInfoResponse\",\n  \"description\": \"MsspLicenseInfoResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-info-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creditsPurchased\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"creditsAllocated\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"balanceCredit\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"numOfTenant\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"endTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\
  \n    },\n    \"msspLicensePoolInfos\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"licensePoolName\": {\n            \"type\": \"string\"\n          },\n          \"licensePoolId\": {\n            \"type\": \"string\"\n          },\n          \"serialNumber\": {\n            \"type\": \"string\"\n          },\n          \"startTime\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"endTime\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"numOfTenant\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          },\n          \"creditsAllocated\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          },\n          \"creditsPurchased\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          },\n          \"tenantGroupLicenseInfos\"\
  : {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"tenantGroupName\": {\n                  \"type\": \"string\"\n                },\n                \"tenantGroupId\": {\n                  \"type\": \"string\"\n                },\n                \"numOfTenant\": {\n                  \"type\": \"integer\",\n                  \"format\": \"int32\"\n                },\n                \"creditsAllocated\": {\n                  \"type\": \"integer\",\n                  \"format\": \"int32\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-info-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MsspLicenseInfoResponse
---

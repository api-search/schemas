---
description: 'MsspLicensePoolRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: MsspLicensePoolRequest
properties_list:
- description: ''
  name: serialNumber
  type: string
- description: ''
  name: poolName
  type: string
- description: ''
  name: startDate
  type: integer
- description: ''
  name: endDate
  type: integer
- description: ''
  name: credits
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-mssp-license-pool-request-schema.json
slug: prisma-cloud-mssp-api-mssp-license-pool-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MsspLicensePoolRequest\",\n  \"description\": \"MsspLicensePoolRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-pool-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serialNumber\": {\n      \"type\": \"string\"\n    },\n    \"poolName\": {\n      \"maxLength\": 63,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"startDate\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"endDate\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"credits\": {\n      \"minimum\": 1,\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  },\n  \"required\": [\n    \"credits\",\n    \"endDate\",\n    \"poolName\",\n    \"serialNumber\"\
  ,\n    \"startDate\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-pool-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MsspLicensePoolRequest
---

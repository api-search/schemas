---
description: 'LicenseInfo schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: LicenseInfo
properties_list:
- description: ''
  name: licensePoolId
  type: string
- description: ''
  name: allocatedCredits
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-license-info-schema.json
slug: prisma-cloud-mssp-api-license-info
source_filename: prisma-cloud-mssp-api-license-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LicenseInfo\",\n  \"description\": \"LicenseInfo schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-license-info-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"licensePoolId\": {\n      \"type\": \"string\"\n    },\n    \"allocatedCredits\": {\n      \"minimum\": 1,\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    }\n  },\n  \"required\": [\n    \"allocatedCredits\",\n    \"licensePoolId\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-license-info-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: LicenseInfo
---

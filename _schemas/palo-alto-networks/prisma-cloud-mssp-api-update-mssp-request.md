---
description: 'UpdateMsspRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: UpdateMsspRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: addLicensePool
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-update-mssp-request-schema.json
slug: prisma-cloud-mssp-api-update-mssp-request
source_filename: prisma-cloud-mssp-api-update-mssp-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateMsspRequest\",\n  \"description\": \"UpdateMsspRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-update-mssp-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"maxLength\": 63,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"addLicensePool\": {\n      \"required\": [\n        \"credits\",\n        \"endDate\",\n        \"poolName\",\n        \"serialNumber\",\n        \"startDate\"\n      ],\n      \"type\": \"object\",\n      \"properties\": {\n        \"serialNumber\": {\n          \"type\": \"string\"\n        },\n        \"poolName\": {\n          \"maxLength\": 63,\n          \"minLength\": 3,\n          \"type\": \"string\"\n        },\n        \"startDate\":\
  \ {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"endDate\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"credits\": {\n          \"minimum\": 1,\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-update-mssp-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: UpdateMsspRequest
---

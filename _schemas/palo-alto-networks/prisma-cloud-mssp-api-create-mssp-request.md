---
description: 'CreateMsspRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: CreateMsspRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: customerSupportId
  type: string
- description: ''
  name: contactInfo
  type: object
- description: ''
  name: licensePool
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-create-mssp-request-schema.json
slug: prisma-cloud-mssp-api-create-mssp-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateMsspRequest\",\n  \"description\": \"CreateMsspRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-create-mssp-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"maxLength\": 63,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"customerSupportId\": {\n      \"type\": \"string\"\n    },\n    \"contactInfo\": {\n      \"required\": [\n        \"email\",\n        \"firstName\",\n        \"lastName\"\n      ],\n      \"type\": \"object\",\n      \"properties\": {\n        \"firstName\": {\n          \"maxLength\": 63,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        },\n        \"lastName\": {\n          \"maxLength\": 63,\n          \"minLength\": 1,\n\
  \          \"type\": \"string\"\n        },\n        \"email\": {\n          \"maxLength\": 128,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"licensePool\": {\n      \"required\": [\n        \"credits\",\n        \"endDate\",\n        \"poolName\",\n        \"serialNumber\",\n        \"startDate\"\n      ],\n      \"type\": \"object\",\n      \"properties\": {\n        \"serialNumber\": {\n          \"type\": \"string\"\n        },\n        \"poolName\": {\n          \"maxLength\": 63,\n          \"minLength\": 3,\n          \"type\": \"string\"\n        },\n        \"startDate\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"endDate\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"credits\": {\n          \"minimum\": 1,\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"\
  contactInfo\",\n    \"customerSupportId\",\n    \"licensePool\",\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-create-mssp-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CreateMsspRequest
---

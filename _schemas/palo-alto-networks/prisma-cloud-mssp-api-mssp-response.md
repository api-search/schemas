---
description: 'MsspResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: MsspResponse
properties_list:
- description: ''
  name: msspId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: createdBy
  type: string
- description: ''
  name: createdAt
  type: integer
- description: ''
  name: customerSupportId
  type: string
- description: ''
  name: contactInfo
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-mssp-response-schema.json
slug: prisma-cloud-mssp-api-mssp-response
source_filename: prisma-cloud-mssp-api-mssp-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MsspResponse\",\n  \"description\": \"MsspResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"msspId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"customerSupportId\": {\n      \"type\": \"string\"\n    },\n    \"contactInfo\": {\n      \"required\": [\n        \"email\",\n        \"firstName\",\n        \"lastName\"\n      ],\n      \"type\": \"object\",\n      \"properties\": {\n        \"firstName\": {\n          \"maxLength\": 63,\n          \"minLength\"\
  : 1,\n          \"type\": \"string\"\n        },\n        \"lastName\": {\n          \"maxLength\": 63,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        },\n        \"email\": {\n          \"maxLength\": 128,\n          \"minLength\": 1,\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MsspResponse
---

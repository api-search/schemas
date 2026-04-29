---
description: 'ContactInfo schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: ContactInfo
properties_list:
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: email
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-contact-info-schema.json
slug: prisma-cloud-mssp-api-contact-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactInfo\",\n  \"description\": \"ContactInfo schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-contact-info-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"maxLength\": 63,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"maxLength\": 63,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"maxLength\": 128,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"email\",\n    \"firstName\",\n    \"lastName\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-contact-info-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ContactInfo
---

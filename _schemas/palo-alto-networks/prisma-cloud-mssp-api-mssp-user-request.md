---
description: 'MsspUserRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: MsspUserRequest
properties_list:
- description: User name of the user.
  name: username
  type: string
- description: First name of the user.
  name: firstName
  type: string
- description: Last name of the user.
  name: lastName
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-mssp-user-request-schema.json
slug: prisma-cloud-mssp-api-mssp-user-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MsspUserRequest\",\n  \"description\": \"MsspUserRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-user-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"maxLength\": 128,\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"User name of the user.\"\n    },\n    \"firstName\": {\n      \"maxLength\": 63,\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"First name of the user.\"\n    },\n    \"lastName\": {\n      \"maxLength\": 63,\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Last name of the user.\"\n    }\n  },\n  \"required\": [\n    \"firstName\",\n    \"lastName\",\n    \"username\"\n\
  \  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-user-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MsspUserRequest
---

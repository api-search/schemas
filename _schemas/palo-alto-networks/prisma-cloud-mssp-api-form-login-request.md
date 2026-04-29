---
description: 'FormLoginRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: FormLoginRequest
properties_list:
- description: username of the user
  name: username
  type: string
- description: password of the user
  name: password
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-form-login-request-schema.json
slug: prisma-cloud-mssp-api-form-login-request
source_filename: prisma-cloud-mssp-api-form-login-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FormLoginRequest\",\n  \"description\": \"FormLoginRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-form-login-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"username of the user\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"password of the user\"\n    }\n  },\n  \"required\": [\n    \"password\",\n    \"username\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-form-login-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: FormLoginRequest
---

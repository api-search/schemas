---
description: 'JwkResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: JwkResponse
properties_list:
- description: ''
  name: kid
  type: string
- description: ''
  name: kty
  type: string
- description: ''
  name: alg
  type: string
- description: ''
  name: key_ops
  type: array
- description: ''
  name: e
  type: string
- description: ''
  name: n
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-jwk-response-schema.json
slug: prisma-cloud-mssp-api-jwk-response
source_filename: prisma-cloud-mssp-api-jwk-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JwkResponse\",\n  \"description\": \"JwkResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-jwk-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kid\": {\n      \"type\": \"string\"\n    },\n    \"kty\": {\n      \"type\": \"string\"\n    },\n    \"alg\": {\n      \"type\": \"string\"\n    },\n    \"key_ops\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"e\": {\n      \"type\": \"string\"\n    },\n    \"n\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"alg\",\n    \"key_ops\",\n    \"kid\",\n    \"kty\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-jwk-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: JwkResponse
---

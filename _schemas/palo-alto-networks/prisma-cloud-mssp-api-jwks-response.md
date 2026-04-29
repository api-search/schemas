---
description: 'JwksResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: JwksResponse
properties_list:
- description: ''
  name: keys
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-jwks-response-schema.json
slug: prisma-cloud-mssp-api-jwks-response
source_filename: prisma-cloud-mssp-api-jwks-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JwksResponse\",\n  \"description\": \"JwksResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-jwks-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keys\": {\n      \"uniqueItems\": true,\n      \"type\": \"array\",\n      \"items\": {\n        \"required\": [\n          \"alg\",\n          \"key_ops\",\n          \"kid\",\n          \"kty\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"kid\": {\n            \"type\": \"string\"\n          },\n          \"kty\": {\n            \"type\": \"string\"\n          },\n          \"alg\": {\n            \"type\": \"string\"\n          },\n          \"key_ops\": {\n            \"type\": \"array\",\n            \"items\": {\n     \
  \         \"type\": \"string\"\n            }\n          },\n          \"e\": {\n            \"type\": \"string\"\n          },\n          \"n\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"keys\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-jwks-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: JwksResponse
---

---
description: 'OperationAckRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: OperationAckRequest
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: errorMessage
  type: string
- description: ''
  name: tenantUpdate
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-operation-ack-request-schema.json
slug: prisma-cloud-mssp-api-operation-ack-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OperationAckRequest\",\n  \"description\": \"OperationAckRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-operation-ack-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SUCCESS\",\n        \"FAILURE\"\n      ]\n    },\n    \"errorMessage\": {\n      \"type\": \"string\"\n    },\n    \"tenantUpdate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"prismaId\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"externalTenantId\": {\n          \"type\": \"string\"\n        },\n        \"stackName\": {\n          \"type\": \"string\"\n        },\n        \"stackBaseUrl\": {\n     \
  \     \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-operation-ack-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: OperationAckRequest
---

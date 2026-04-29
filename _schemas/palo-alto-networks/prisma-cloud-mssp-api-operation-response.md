---
description: 'OperationResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: OperationResponse
properties_list:
- description: ''
  name: requestId
  type: string
- description: ''
  name: msspId
  type: string
- description: ''
  name: operationType
  type: string
- description: ''
  name: operationName
  type: string
- description: ''
  name: operationDescription
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: tenantChanges
  type: array
- description: ''
  name: startedBy
  type: string
- description: ''
  name: startedAt
  type: integer
- description: ''
  name: updatedAt
  type: integer
- description: ''
  name: isRetryable
  type: boolean
- description: ''
  name: retryOf
  type: string
- description: ''
  name: retriedBy
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-operation-response-schema.json
slug: prisma-cloud-mssp-api-operation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OperationResponse\",\n  \"description\": \"OperationResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-operation-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"msspId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"operationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MESSAGE_FAN_OUT\",\n        \"ORCHESTRATOR_REQUEST\"\n      ]\n    },\n    \"operationName\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PROVISION_TENANT\",\n        \"UPDATE_TENANT\",\n        \"DELETE_TENANT\",\n        \"OFFBOARD_TENANT\",\n        \"REPLICATE_ACTION\",\n        \"CREATE_USER\"\
  ,\n        \"UPDATE_USER\",\n        \"DELETE_USER\",\n        \"POLICY_MAP\",\n        \"POLICY_UNMAP\",\n        \"SYNC_POLICIES\"\n      ]\n    },\n    \"operationDescription\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IN_PROGRESS\",\n        \"SUCCESS\",\n        \"FAILURE\"\n      ]\n    },\n    \"tenantChanges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"tenantChangeId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"externalTenantId\": {\n            \"type\": \"string\"\n          },\n          \"tenantPrismaId\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"IN_PROGRESS\",\n              \"SUCCESS\",\n              \"FAILURE\"\n            ]\n          },\n          \"updatedAt\"\
  : {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          }\n        }\n      }\n    },\n    \"startedBy\": {\n      \"type\": \"string\"\n    },\n    \"startedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"updatedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"isRetryable\": {\n      \"type\": \"boolean\"\n    },\n    \"retryOf\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"retriedBy\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-operation-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: OperationResponse
---

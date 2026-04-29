---
description: 'OperationsResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: OperationsResponse
properties_list:
- description: ''
  name: value
  type: array
- description: ''
  name: nextPageToken
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-operations-response-schema.json
slug: prisma-cloud-mssp-api-operations-response
source_filename: prisma-cloud-mssp-api-operations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OperationsResponse\",\n  \"description\": \"OperationsResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-operations-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"requestId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"msspId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"operationType\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"MESSAGE_FAN_OUT\",\n              \"ORCHESTRATOR_REQUEST\"\n            ]\n          },\n          \"operationName\"\
  : {\n            \"type\": \"string\",\n            \"enum\": [\n              \"PROVISION_TENANT\",\n              \"UPDATE_TENANT\",\n              \"DELETE_TENANT\",\n              \"OFFBOARD_TENANT\",\n              \"REPLICATE_ACTION\",\n              \"CREATE_USER\",\n              \"UPDATE_USER\",\n              \"DELETE_USER\",\n              \"POLICY_MAP\",\n              \"POLICY_UNMAP\",\n              \"SYNC_POLICIES\"\n            ]\n          },\n          \"operationDescription\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"IN_PROGRESS\",\n              \"SUCCESS\",\n              \"FAILURE\"\n            ]\n          },\n          \"tenantChanges\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"tenantChangeId\": {\n                  \"type\": \"string\",\n    \
  \              \"format\": \"uuid\"\n                },\n                \"externalTenantId\": {\n                  \"type\": \"string\"\n                },\n                \"tenantPrismaId\": {\n                  \"type\": \"string\"\n                },\n                \"status\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"IN_PROGRESS\",\n                    \"SUCCESS\",\n                    \"FAILURE\"\n                  ]\n                },\n                \"updatedAt\": {\n                  \"type\": \"integer\",\n                  \"format\": \"int64\"\n                }\n              }\n            }\n          },\n          \"startedBy\": {\n            \"type\": \"string\"\n          },\n          \"startedAt\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"updatedAt\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n         \
  \ \"isRetryable\": {\n            \"type\": \"boolean\"\n          },\n          \"retryOf\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"retriedBy\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        }\n      }\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-operations-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: OperationsResponse
---

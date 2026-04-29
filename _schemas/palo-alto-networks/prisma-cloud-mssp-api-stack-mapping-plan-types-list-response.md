---
description: 'StackMappingPlanTypesListResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: StackMappingPlanTypesListResponse
properties_list:
- description: ''
  name: stackMappings
  type: array
- description: ''
  name: planTypes
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-stack-mapping-plan-types-list-response-schema.json
slug: prisma-cloud-mssp-api-stack-mapping-plan-types-list-response
source_filename: prisma-cloud-mssp-api-stack-mapping-plan-types-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StackMappingPlanTypesListResponse\",\n  \"description\": \"StackMappingPlanTypesListResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-stack-mapping-plan-types-list-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stackMappings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"displayName\": {\n            \"type\": \"string\"\n          },\n          \"apiHost\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"planTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-stack-mapping-plan-types-list-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: StackMappingPlanTypesListResponse
---

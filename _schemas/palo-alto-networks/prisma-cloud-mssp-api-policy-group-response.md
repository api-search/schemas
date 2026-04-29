---
description: 'PolicyGroupResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: PolicyGroupResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: policies
  type: array
- description: ''
  name: tenantGroups
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-policy-group-response-schema.json
slug: prisma-cloud-mssp-api-policy-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyGroupResponse\",\n  \"description\": \"PolicyGroupResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-policy-group-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"policies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tenantGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"tenantGroupId\": {\n            \"type\": \"string\",\n \
  \           \"format\": \"uuid\"\n          },\n          \"tenantGroupName\": {\n            \"type\": \"string\"\n          },\n          \"tenantCount\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-policy-group-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PolicyGroupResponse
---

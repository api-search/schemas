---
description: 'PolicyGroupsListResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: PolicyGroupsListResponse
properties_list:
- description: ''
  name: value
  type: array
- description: ''
  name: nextPageToken
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-policy-groups-list-response-schema.json
slug: prisma-cloud-mssp-api-policy-groups-list-response
source_filename: prisma-cloud-mssp-api-policy-groups-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyGroupsListResponse\",\n  \"description\": \"PolicyGroupsListResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-policy-groups-list-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"policyCount\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          },\n          \"tenantGroupCount\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\"\n          }\n   \
  \     }\n      }\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-policy-groups-list-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PolicyGroupsListResponse
---

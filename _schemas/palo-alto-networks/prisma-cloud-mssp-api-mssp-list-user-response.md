---
description: 'MsspListUserResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: MsspListUserResponse
properties_list:
- description: ''
  name: value
  type: array
- description: ''
  name: nextPageToken
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-mssp-list-user-response-schema.json
slug: prisma-cloud-mssp-api-mssp-list-user-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MsspListUserResponse\",\n  \"description\": \"MsspListUserResponse schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-list-user-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"username\": {\n            \"type\": \"string\"\n          },\n          \"firstName\": {\n            \"type\": \"string\"\n          },\n          \"lastName\": {\n            \"type\": \"string\"\n          },\n          \"lastModifiedBy\": {\n            \"type\": \"string\"\n          },\n          \"lastModifiedAt\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          }\n\
  \        }\n      }\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-list-user-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MsspListUserResponse
---

---
description: 'RelativeTimeDuration schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: RelativeTimeDuration
properties_list:
- description: ''
  name: unit
  type: string
- description: Number of time units
  name: amount
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-relative-time-duration-schema.json
slug: prisma-cloud-mssp-api-relative-time-duration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RelativeTimeDuration\",\n  \"description\": \"RelativeTimeDuration schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-relative-time-duration-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unit\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"week\",\n        \"month\",\n        \"year\"\n      ]\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of time units\",\n      \"format\": \"int32\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-relative-time-duration-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RelativeTimeDuration
---

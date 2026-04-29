---
description: AlertFilter schema from Palo Alto Networks Prisma Cloud CSPM API
layout: schema
name: AlertFilter
properties_list:
- description: Filter field name (e.g., alert.status, cloud.type, policy.severity, cloud.accountId).
  name: name
  type: string
- description: ''
  name: operator
  type: string
- description: ''
  name: value
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-cspm-api-alert-filter-schema.json
slug: prisma-cloud-cspm-api-alert-filter
source_filename: prisma-cloud-cspm-api-alert-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlertFilter\",\n  \"description\": \"AlertFilter schema from Palo Alto Networks Prisma Cloud CSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-alert-filter-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Filter field name (e.g., alert.status, cloud.type, policy.severity, cloud.accountId).\"\n    },\n    \"operator\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"=\"\n      ]\n    },\n    \"value\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-alert-filter-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AlertFilter
---

---
description: TimeRange schema from Palo Alto Networks Prisma Cloud CSPM API
layout: schema
name: TimeRange
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: value
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-cspm-api-time-range-schema.json
slug: prisma-cloud-cspm-api-time-range
source_filename: prisma-cloud-cspm-api-time-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeRange\",\n  \"description\": \"TimeRange schema from Palo Alto Networks Prisma Cloud CSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-time-range-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"relative\",\n        \"absolute\",\n        \"to_now\"\n      ]\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"integer\"\n        },\n        \"unit\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"minute\",\n            \"hour\",\n            \"day\",\n            \"week\",\n            \"month\",\n            \"year\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-time-range-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: TimeRange
---

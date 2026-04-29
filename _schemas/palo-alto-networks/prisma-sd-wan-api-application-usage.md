---
description: ApplicationUsage schema from Palo Alto Networks Prisma SD-WAN API
layout: schema
name: ApplicationUsage
properties_list:
- description: Application name.
  name: application
  type: string
- description: Site where the application traffic was observed.
  name: site_id
  type: string
- description: Uploaded bytes for the application.
  name: bytes_up
  type: integer
- description: Downloaded bytes for the application.
  name: bytes_down
  type: integer
- description: Number of application sessions.
  name: sessions
  type: integer
- description: Average latency for application traffic.
  name: avg_latency_ms
  type: number
- description: Time bucket for the usage data.
  name: timestamp
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-sd-wan-api-application-usage-schema.json
slug: prisma-sd-wan-api-application-usage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationUsage\",\n  \"description\": \"ApplicationUsage schema from Palo Alto Networks Prisma SD-WAN API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-application-usage-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"string\",\n      \"description\": \"Application name.\"\n    },\n    \"site_id\": {\n      \"type\": \"string\",\n      \"description\": \"Site where the application traffic was observed.\"\n    },\n    \"bytes_up\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Uploaded bytes for the application.\"\n    },\n    \"bytes_down\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Downloaded bytes for the application.\"\n    },\n    \"sessions\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Number of application sessions.\"\n    },\n    \"avg_latency_ms\": {\n      \"type\": \"number\",\n      \"description\": \"Average latency for application traffic.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time bucket for the usage data.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-application-usage-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ApplicationUsage
---

---
description: 'Task schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: Task
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: webhookUrl
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: scheduledTime
  type: integer
- description: ''
  name: submitTime
  type: integer
- description: ''
  name: recur
  type: object
- description: ''
  name: matureTime
  type: integer
- description: ''
  name: cancel
  type: boolean
- description: ''
  name: properties
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-task-schema.json
slug: prisma-cloud-mssp-api-task
source_filename: prisma-cloud-mssp-api-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Task\",\n  \"description\": \"Task schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-task-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"webhookUrl\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"scheduledTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"submitTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"recur\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\"\n        },\n        \"recurString\": {\n          \"type\": \"string\"\n        }\n      }\n\
  \    },\n    \"matureTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"cancel\": {\n      \"type\": \"boolean\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-task-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Task
---

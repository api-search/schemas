---
description: 'ScheduleTaskRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: ScheduleTaskRequest
properties_list:
- description: ''
  name: scheduledTime
  type: integer
- description: ''
  name: prismaIds
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-schedule-task-request-schema.json
slug: prisma-cloud-mssp-api-schedule-task-request
source_filename: prisma-cloud-mssp-api-schedule-task-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScheduleTaskRequest\",\n  \"description\": \"ScheduleTaskRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-schedule-task-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scheduledTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"prismaIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-schedule-task-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ScheduleTaskRequest
---

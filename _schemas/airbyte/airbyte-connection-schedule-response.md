---
description: schedule for when the the connection should run, per the schedule type
layout: schema
name: ConnectionScheduleResponse
properties_list:
- description: ''
  name: scheduleType
  type: object
- description: ''
  name: cronExpression
  type: string
- description: ''
  name: basicTiming
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-connection-schedule-response-schema.json
slug: airbyte-connection-schedule-response
source_filename: airbyte-connection-schedule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connection-schedule-response-schema.json\",\n  \"title\": \"ConnectionScheduleResponse\",\n  \"description\": \"schedule for when the the connection should run, per the schedule type\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scheduleType\": {\n      \"$ref\": \"#/components/schemas/ScheduleTypeWithBasicEnum\"\n    },\n    \"cronExpression\": {\n      \"type\": \"string\"\n    },\n    \"basicTiming\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"scheduleType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connection-schedule-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ConnectionScheduleResponse
---

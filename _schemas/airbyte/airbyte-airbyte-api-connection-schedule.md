---
description: schedule for when the the connection should run, per the schedule type
layout: schema
name: AirbyteApiConnectionSchedule
properties_list:
- description: ''
  name: scheduleType
  type: object
- description: ''
  name: cronExpression
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-airbyte-api-connection-schedule-schema.json
slug: airbyte-airbyte-api-connection-schedule
source_filename: airbyte-airbyte-api-connection-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-airbyte-api-connection-schedule-schema.json\",\n  \"title\": \"AirbyteApiConnectionSchedule\",\n  \"description\": \"schedule for when the the connection should run, per the schedule type\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scheduleType\": {\n      \"$ref\": \"#/components/schemas/ScheduleTypeEnum\"\n    },\n    \"cronExpression\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"scheduleType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-airbyte-api-connection-schedule-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: AirbyteApiConnectionSchedule
---

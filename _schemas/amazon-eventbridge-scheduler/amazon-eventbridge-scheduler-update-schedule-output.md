---
description: UpdateScheduleOutput schema from Amazon EventBridge Scheduler
layout: schema
name: UpdateScheduleOutput
properties_list:
- description: ''
  name: ScheduleArn
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-update-schedule-output-schema.json
slug: amazon-eventbridge-scheduler-update-schedule-output
source_filename: amazon-eventbridge-scheduler-update-schedule-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-update-schedule-output-schema.json\",\n  \"title\": \"UpdateScheduleOutput\",\n  \"description\": \"UpdateScheduleOutput schema from Amazon EventBridge Scheduler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the schedule that you updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScheduleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-update-schedule-output-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: UpdateScheduleOutput
---

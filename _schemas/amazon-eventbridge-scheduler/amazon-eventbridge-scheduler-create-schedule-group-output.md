---
description: CreateScheduleGroupOutput schema from Amazon EventBridge Scheduler
layout: schema
name: CreateScheduleGroupOutput
properties_list:
- description: ''
  name: ScheduleGroupArn
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-create-schedule-group-output-schema.json
slug: amazon-eventbridge-scheduler-create-schedule-group-output
source_filename: amazon-eventbridge-scheduler-create-schedule-group-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-create-schedule-group-output-schema.json\",\n  \"title\": \"CreateScheduleGroupOutput\",\n  \"description\": \"CreateScheduleGroupOutput schema from Amazon EventBridge Scheduler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduleGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleGroupArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the schedule group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScheduleGroupArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-create-schedule-group-output-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: CreateScheduleGroupOutput
---

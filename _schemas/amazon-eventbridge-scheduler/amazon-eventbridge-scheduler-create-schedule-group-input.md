---
description: CreateScheduleGroupInput schema from Amazon EventBridge Scheduler
layout: schema
name: CreateScheduleGroupInput
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-create-schedule-group-input-schema.json
slug: amazon-eventbridge-scheduler-create-schedule-group-input
source_filename: amazon-eventbridge-scheduler-create-schedule-group-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-create-schedule-group-input-schema.json\",\n  \"title\": \"CreateScheduleGroupInput\",\n  \"description\": \"CreateScheduleGroupInput schema from Amazon EventBridge Scheduler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \" Unique, case-sensitive identifier you provide to ensure the idempotency of the request. If you do not specify a client token, EventBridge Scheduler uses a randomly generated token for the request to ensure idempotency. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n   \
  \       \"description\": \"The list of tags to associate with the schedule group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-create-schedule-group-input-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: CreateScheduleGroupInput
---

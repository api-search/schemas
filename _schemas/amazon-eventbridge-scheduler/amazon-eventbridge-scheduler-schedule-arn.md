---
description: ScheduleArn schema from Amazon EventBridge Scheduler
layout: schema
name: ScheduleArn
properties_list: []
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-schedule-arn-schema.json
slug: amazon-eventbridge-scheduler-schedule-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-schedule-arn-schema.json\",\n  \"title\": \"ScheduleArn\",\n  \"description\": \"ScheduleArn schema from Amazon EventBridge Scheduler\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws(-[a-z]+)?:scheduler:[a-z0-9\\\\-]+:\\\\d{12}:schedule\\\\/[0-9a-zA-Z-_.]+\\\\/[0-9a-zA-Z-_.]+$\",\n  \"minLength\": 1,\n  \"maxLength\": 1224\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-schedule-arn-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: ScheduleArn
---

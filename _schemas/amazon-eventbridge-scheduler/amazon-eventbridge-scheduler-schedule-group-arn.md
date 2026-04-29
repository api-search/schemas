---
description: ScheduleGroupArn schema from Amazon EventBridge Scheduler
layout: schema
name: ScheduleGroupArn
properties_list: []
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-schedule-group-arn-schema.json
slug: amazon-eventbridge-scheduler-schedule-group-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-schedule-group-arn-schema.json\",\n  \"title\": \"ScheduleGroupArn\",\n  \"description\": \"ScheduleGroupArn schema from Amazon EventBridge Scheduler\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws(-[a-z]+)?:scheduler:[a-z0-9\\\\-]+:\\\\d{12}:schedule-group\\\\/[0-9a-zA-Z-_.]+$\",\n  \"minLength\": 1,\n  \"maxLength\": 1224\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-schedule-group-arn-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: ScheduleGroupArn
---

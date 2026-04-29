---
description: RoleArn schema from Amazon EventBridge Scheduler
layout: schema
name: RoleArn
properties_list: []
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-role-arn-schema.json
slug: amazon-eventbridge-scheduler-role-arn
source_filename: amazon-eventbridge-scheduler-role-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-role-arn-schema.json\",\n  \"title\": \"RoleArn\",\n  \"description\": \"RoleArn schema from Amazon EventBridge Scheduler\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws(-[a-z]+)?:iam::\\\\d{12}:role\\\\/[\\\\w+=,.@\\\\/-]+$\",\n  \"minLength\": 1,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-role-arn-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: RoleArn
---

---
description: DeadLetterConfigArnString schema from Amazon EventBridge Scheduler
layout: schema
name: DeadLetterConfigArnString
properties_list: []
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-dead-letter-config-arn-string-schema.json
slug: amazon-eventbridge-scheduler-dead-letter-config-arn-string
source_filename: amazon-eventbridge-scheduler-dead-letter-config-arn-string-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-dead-letter-config-arn-string-schema.json\",\n  \"title\": \"DeadLetterConfigArnString\",\n  \"description\": \"DeadLetterConfigArnString schema from Amazon EventBridge Scheduler\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws(-[a-z]+)?:sqs:[a-z0-9\\\\-]+:\\\\d{12}:[a-zA-Z0-9\\\\-_]+$\",\n  \"minLength\": 1,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-dead-letter-config-arn-string-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: DeadLetterConfigArnString
---

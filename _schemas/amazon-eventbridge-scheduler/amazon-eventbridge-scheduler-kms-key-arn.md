---
description: KmsKeyArn schema from Amazon EventBridge Scheduler
layout: schema
name: KmsKeyArn
properties_list: []
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-kms-key-arn-schema.json
slug: amazon-eventbridge-scheduler-kms-key-arn
source_filename: amazon-eventbridge-scheduler-kms-key-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-kms-key-arn-schema.json\",\n  \"title\": \"KmsKeyArn\",\n  \"description\": \"KmsKeyArn schema from Amazon EventBridge Scheduler\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws(-[a-z]+)?:kms:[a-z0-9\\\\-]+:\\\\d{12}:(key|alias)\\\\/[0-9a-zA-Z-_]*$\",\n  \"minLength\": 1,\n  \"maxLength\": 2048\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-kms-key-arn-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: KmsKeyArn
---

---
description: PipeArn schema from Amazon EventBridge Pipes
layout: schema
name: PipeArn
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-arn-schema.json
slug: amazon-eventbridge-pipes-pipe-arn
source_filename: amazon-eventbridge-pipes-pipe-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-arn-schema.json\",\n  \"title\": \"PipeArn\",\n  \"description\": \"PipeArn schema from Amazon EventBridge Pipes\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws([a-z]|\\\\-)*:([a-zA-Z0-9\\\\-]+):([a-z]|\\\\d|\\\\-)*:([0-9]{12})?:(.+)$\",\n  \"minLength\": 1,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-arn-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeArn
---

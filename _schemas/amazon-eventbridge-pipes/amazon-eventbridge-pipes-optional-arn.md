---
description: OptionalArn schema from Amazon EventBridge Pipes
layout: schema
name: OptionalArn
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-optional-arn-schema.json
slug: amazon-eventbridge-pipes-optional-arn
source_filename: amazon-eventbridge-pipes-optional-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-optional-arn-schema.json\",\n  \"title\": \"OptionalArn\",\n  \"description\": \"OptionalArn schema from Amazon EventBridge Pipes\",\n  \"type\": \"string\",\n  \"pattern\": \"^$|arn:(aws[a-zA-Z0-9-]*):([a-zA-Z0-9\\\\-]+):([a-z]{2}((-gov)|(-iso(b?)))?-[a-z]+-\\\\d{1})?:(\\\\d{12})?:(.+)$\",\n  \"minLength\": 0,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-optional-arn-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: OptionalArn
---

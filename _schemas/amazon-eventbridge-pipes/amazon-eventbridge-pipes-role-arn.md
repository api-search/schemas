---
description: RoleArn schema from Amazon EventBridge Pipes
layout: schema
name: RoleArn
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-role-arn-schema.json
slug: amazon-eventbridge-pipes-role-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-role-arn-schema.json\",\n  \"title\": \"RoleArn\",\n  \"description\": \"RoleArn schema from Amazon EventBridge Pipes\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:(aws[a-zA-Z-]*)?:iam::\\\\d{12}:role/?[a-zA-Z0-9+=,.@\\\\-_/]+$\",\n  \"minLength\": 1,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-role-arn-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: RoleArn
---

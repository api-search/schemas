---
description: // Optional SecretManager ARN which stores the database credentials
layout: schema
name: SecretManagerArn
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-secret-manager-arn-schema.json
slug: amazon-eventbridge-pipes-secret-manager-arn
source_filename: amazon-eventbridge-pipes-secret-manager-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-secret-manager-arn-schema.json\",\n  \"title\": \"SecretManagerArn\",\n  \"description\": \"// Optional SecretManager ARN which stores the database credentials\",\n  \"type\": \"string\",\n  \"pattern\": \"^(^arn:aws([a-z]|\\\\-)*:secretsmanager:([a-z]{2}((-gov)|(-iso(b?)))?-[a-z]+-\\\\d{1}):(\\\\d{12}):secret:.+)$\",\n  \"minLength\": 1,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-secret-manager-arn-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: SecretManagerArn
---

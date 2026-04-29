---
description: // For targets, can either specify an ARN or a jsonpath pointing to the ARN.
layout: schema
name: SecretManagerArnOrJsonPath
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-secret-manager-arn-or-json-path-schema.json
slug: amazon-eventbridge-pipes-secret-manager-arn-or-json-path
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-secret-manager-arn-or-json-path-schema.json\",\n  \"title\": \"SecretManagerArnOrJsonPath\",\n  \"description\": \"// For targets, can either specify an ARN or a jsonpath pointing to the ARN.\",\n  \"type\": \"string\",\n  \"pattern\": \"^(^arn:aws([a-z]|\\\\-)*:secretsmanager:([a-z]{2}((-gov)|(-iso(b?)))?-[a-z]+-\\\\d{1}):(\\\\d{12}):secret:.+)|(\\\\$(\\\\.[\\\\w/_-]+(\\\\[(\\\\d+|\\\\*)\\\\])*)*)$\",\n  \"minLength\": 1,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-secret-manager-arn-or-json-path-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: SecretManagerArnOrJsonPath
---

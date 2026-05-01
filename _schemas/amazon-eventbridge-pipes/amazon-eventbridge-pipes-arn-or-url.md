---
description: ArnOrUrl schema from Amazon EventBridge Pipes
layout: schema
name: ArnOrUrl
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-arn-or-url-schema.json
slug: amazon-eventbridge-pipes-arn-or-url
source_filename: amazon-eventbridge-pipes-arn-or-url-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-arn-or-url-schema.json\",\n  \"title\": \"ArnOrUrl\",\n  \"description\": \"ArnOrUrl schema from Amazon EventBridge Pipes\",\n  \"type\": \"string\",\n  \"pattern\": \"^smk://(([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9\\\\-]*[a-zA-Z0-9])\\\\.)*([A-Za-z0-9]|[A-Za-z0-9][A-Za-z0-9\\\\-]*[A-Za-z0-9]):[0-9]{1,5}|arn:(aws[a-zA-Z0-9-]*):([a-zA-Z0-9\\\\-]+):([a-z]{2}((-gov)|(-iso(b?)))?-[a-z]+-\\\\d{1})?:(\\\\d{12})?:(.+)$\",\n  \"minLength\": 1,\n  \"maxLength\": 1600\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-arn-or-url-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: ArnOrUrl
---

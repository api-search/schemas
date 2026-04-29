---
description: HeaderValue schema from Amazon EventBridge Pipes
layout: schema
name: HeaderValue
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-header-value-schema.json
slug: amazon-eventbridge-pipes-header-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-header-value-schema.json\",\n  \"title\": \"HeaderValue\",\n  \"description\": \"HeaderValue schema from Amazon EventBridge Pipes\",\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"^[ \\\\t]*[\\\\x20-\\\\x7E]+([ \\\\t]+[\\\\x20-\\\\x7E]+)*[ \\\\t]*|(\\\\$(\\\\.[\\\\w/_-]+(\\\\[(\\\\d+|\\\\*)\\\\])*)*)$\",\n  \"minLength\": 0,\n  \"maxLength\": 512\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-header-value-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: HeaderValue
---

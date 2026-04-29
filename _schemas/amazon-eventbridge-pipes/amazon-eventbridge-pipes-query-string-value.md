---
description: QueryStringValue schema from Amazon EventBridge Pipes
layout: schema
name: QueryStringValue
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-query-string-value-schema.json
slug: amazon-eventbridge-pipes-query-string-value
source_filename: amazon-eventbridge-pipes-query-string-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-query-string-value-schema.json\",\n  \"title\": \"QueryStringValue\",\n  \"description\": \"QueryStringValue schema from Amazon EventBridge Pipes\",\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"^[^\\\\x00-\\\\x09\\\\x0B\\\\x0C\\\\x0E-\\\\x1F\\\\x7F]+|(\\\\$(\\\\.[\\\\w/_-]+(\\\\[(\\\\d+|\\\\*)\\\\])*)*)$\",\n  \"minLength\": 0,\n  \"maxLength\": 512\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-query-string-value-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: QueryStringValue
---

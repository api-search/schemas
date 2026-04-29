---
description: SecurityGroup schema from Amazon EventBridge Pipes
layout: schema
name: SecurityGroup
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-security-group-schema.json
slug: amazon-eventbridge-pipes-security-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-security-group-schema.json\",\n  \"title\": \"SecurityGroup\",\n  \"description\": \"SecurityGroup schema from Amazon EventBridge Pipes\",\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"^sg-[0-9a-zA-Z]*|(\\\\$(\\\\.[\\\\w/_-]+(\\\\[(\\\\d+|\\\\*)\\\\])*)*)$\",\n  \"minLength\": 1,\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-security-group-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: SecurityGroup
---

---
description: Subnet schema from Amazon EventBridge Pipes
layout: schema
name: Subnet
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-subnet-schema.json
slug: amazon-eventbridge-pipes-subnet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-subnet-schema.json\",\n  \"title\": \"Subnet\",\n  \"description\": \"Subnet schema from Amazon EventBridge Pipes\",\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"^subnet-[0-9a-z]*|(\\\\$(\\\\.[\\\\w/_-]+(\\\\[(\\\\d+|\\\\*)\\\\])*)*)$\",\n  \"minLength\": 1,\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-subnet-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: Subnet
---

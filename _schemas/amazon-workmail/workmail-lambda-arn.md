---
description: LambdaArn schema from Amazon WorkMail API
layout: schema
name: LambdaArn
properties_list: []
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-lambda-arn-schema.json
slug: workmail-lambda-arn
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws:lambda:[a-z]{2}-[a-z]+-\\\\d{1}:\\\\d{12}:function:[a-zA-Z0-9\\\\-_\\\\.]+(:(\\\\$LATEST|[a-zA-Z0-9\\\\-_]+))?\",\n  \"minLength\": 49,\n  \"maxLength\": 256,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LambdaArn\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-lambda-arn-schema.json\",\n  \"description\": \"LambdaArn schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-lambda-arn-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: LambdaArn
---

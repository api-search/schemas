---
description: Kinesis stream ARN to which log events are published.
layout: schema
name: KinesisStreamArn
properties_list: []
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-kinesis-stream-arn-schema.json
slug: workspaces-web-kinesis-stream-arn
source_filename: workspaces-web-kinesis-stream-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"arn:[\\\\w+=/,.@-]+:kinesis:[a-zA-Z0-9\\\\-]*:[a-zA-Z0-9]{1,12}:stream/.+\",\n  \"description\": \"Kinesis stream ARN to which log events are published.\",\n  \"minLength\": 20,\n  \"maxLength\": 2048,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KinesisStreamArn\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-kinesis-stream-arn-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-kinesis-stream-arn-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: KinesisStreamArn
---

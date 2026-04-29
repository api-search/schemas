---
description: ''
layout: schema
name: TagResourceInput
properties_list:
- description: The ARN of the CloudWatch resource that you're adding tags to.
  name: ResourceARN
  type: string
- description: The list of key-value pairs to associate with the alarm.
  name: Tags
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-tag-resource-input-schema.json
slug: cloudwatch-tag-resource-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagResourceInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the CloudWatch resource that you're adding tags to.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"The list of key-value pairs to associate with the alarm.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-tag-resource-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: TagResourceInput
---

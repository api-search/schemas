---
description: ''
layout: schema
name: UntagResourceInput
properties_list:
- description: The ARN of the CloudWatch resource that you're removing tags from.
  name: ResourceARN
  type: string
- description: The list of tag keys to remove from the resource.
  name: TagKeys
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-untag-resource-input-schema.json
slug: cloudwatch-untag-resource-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UntagResourceInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the CloudWatch resource that you're removing tags from.\"\n    },\n    \"TagKeys\": {\n      \"type\": \"array\",\n      \"description\": \"The list of tag keys to remove from the resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-untag-resource-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: UntagResourceInput
---

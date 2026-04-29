---
description: ''
layout: schema
name: ListTagsForResourceInput
properties_list:
- description: The ARN of the CloudWatch resource that you want to view tags for.
  name: ResourceARN
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-list-tags-for-resource-input-schema.json
slug: cloudwatch-list-tags-for-resource-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTagsForResourceInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the CloudWatch resource that you want to view tags for.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-list-tags-for-resource-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: ListTagsForResourceInput
---

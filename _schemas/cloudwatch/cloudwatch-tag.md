---
description: A key-value pair associated with a CloudWatch resource.
layout: schema
name: Tag
properties_list:
- description: A string that you can use to assign a value.
  name: Key
  type: string
- description: The value for the specified tag key.
  name: Value
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-tag-schema.json
slug: cloudwatch-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"type\": \"object\",\n  \"description\": \"A key-value pair associated with a CloudWatch resource.\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"A string that you can use to assign a value.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The value for the specified tag key.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-tag-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: Tag
---

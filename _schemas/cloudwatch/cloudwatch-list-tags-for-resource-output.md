---
description: ''
layout: schema
name: ListTagsForResourceOutput
properties_list:
- description: The list of tag keys and values associated with the resource you specified.
  name: Tags
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-list-tags-for-resource-output-schema.json
slug: cloudwatch-list-tags-for-resource-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTagsForResourceOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"The list of tag keys and values associated with the resource you specified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-list-tags-for-resource-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: ListTagsForResourceOutput
---

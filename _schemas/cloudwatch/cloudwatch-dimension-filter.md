---
description: Represents filters for a dimension.
layout: schema
name: DimensionFilter
properties_list:
- description: The dimension name to be matched.
  name: Name
  type: string
- description: The value of the dimension to be matched.
  name: Value
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-dimension-filter-schema.json
slug: cloudwatch-dimension-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DimensionFilter\",\n  \"type\": \"object\",\n  \"description\": \"Represents filters for a dimension.\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The dimension name to be matched.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the dimension to be matched.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-dimension-filter-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DimensionFilter
---

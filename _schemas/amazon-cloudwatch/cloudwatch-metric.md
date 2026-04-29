---
description: Represents a specific metric
layout: schema
name: Metric
properties_list:
- description: The namespace of the metric
  name: namespace
  type: string
- description: The name of the metric
  name: metricName
  type: string
- description: The dimensions for the metric
  name: dimensions
  type: array
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-metric-schema.json
slug: cloudwatch-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-schema.json\",\n  \"title\": \"Metric\",\n  \"description\": \"Represents a specific metric\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the metric\"\n    },\n    \"metricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric\"\n    },\n    \"dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The dimensions for the metric\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the dimension\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The value of the\
  \ dimension\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: Metric
---

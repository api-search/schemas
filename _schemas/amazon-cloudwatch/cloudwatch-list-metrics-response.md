---
description: Response from the ListMetrics action
layout: schema
name: ListMetricsResponse
properties_list:
- description: The metrics that match the filter criteria
  name: metrics
  type: array
- description: Token for the next page of results
  name: nextToken
  type: string
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-list-metrics-response-schema.json
slug: cloudwatch-list-metrics-response
source_filename: cloudwatch-list-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-list-metrics-response-schema.json\",\n  \"title\": \"ListMetricsResponse\",\n  \"description\": \"Response from the ListMetrics action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"array\",\n      \"description\": \"The metrics that match the filter criteria\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Metric\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for the next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-list-metrics-response-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: ListMetricsResponse
---

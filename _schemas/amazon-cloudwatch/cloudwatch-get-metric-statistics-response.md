---
description: Response from the GetMetricStatistics action
layout: schema
name: GetMetricStatisticsResponse
properties_list:
- description: A label for the specified metric
  name: label
  type: string
- description: The data points for the specified metric
  name: datapoints
  type: array
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-get-metric-statistics-response-schema.json
slug: cloudwatch-get-metric-statistics-response
source_filename: cloudwatch-get-metric-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-get-metric-statistics-response-schema.json\",\n  \"title\": \"GetMetricStatisticsResponse\",\n  \"description\": \"Response from the GetMetricStatistics action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"A label for the specified metric\"\n    },\n    \"datapoints\": {\n      \"type\": \"array\",\n      \"description\": \"The data points for the specified metric\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The time stamp for the data point\"\n          },\n          \"sampleCount\": {\n            \"type\": \"number\",\n            \"description\"\
  : \"The number of metric values\"\n          },\n          \"average\": {\n            \"type\": \"number\",\n            \"description\": \"The average of the metric values\"\n          },\n          \"sum\": {\n            \"type\": \"number\",\n            \"description\": \"The sum of the metric values\"\n          },\n          \"minimum\": {\n            \"type\": \"number\",\n            \"description\": \"The minimum metric value\"\n          },\n          \"maximum\": {\n            \"type\": \"number\",\n            \"description\": \"The maximum metric value\"\n          },\n          \"unit\": {\n            \"type\": \"string\",\n            \"description\": \"The standard unit for the data point\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-get-metric-statistics-response-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: GetMetricStatisticsResponse
---

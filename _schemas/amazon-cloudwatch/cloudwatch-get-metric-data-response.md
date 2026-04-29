---
description: Response from the GetMetricData action
layout: schema
name: GetMetricDataResponse
properties_list:
- description: The metrics that are returned
  name: metricDataResults
  type: array
- description: Token for the next page of results
  name: nextToken
  type: string
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-get-metric-data-response-schema.json
slug: cloudwatch-get-metric-data-response
source_filename: cloudwatch-get-metric-data-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-get-metric-data-response-schema.json\",\n  \"title\": \"GetMetricDataResponse\",\n  \"description\": \"Response from the GetMetricData action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricDataResults\": {\n      \"type\": \"array\",\n      \"description\": \"The metrics that are returned\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The short name specified in the query\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"The human-readable label for the metric\"\n          },\n          \"timestamps\": {\n            \"type\": \"array\",\n            \"description\": \"The timestamps for the data points\"\
  ,\n            \"items\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            }\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"description\": \"The data point values\",\n            \"items\": {\n              \"type\": \"number\"\n            }\n          },\n          \"statusCode\": {\n            \"type\": \"string\",\n            \"description\": \"The status of the returned data\",\n            \"enum\": [\n              \"Complete\",\n              \"InternalError\",\n              \"PartialData\",\n              \"Forbidden\"\n            ]\n          }\n        }\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for the next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-get-metric-data-response-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: GetMetricDataResponse
---

---
description: ''
layout: schema
name: GetMetricDataInput
properties_list:
- description: The metric queries to be returned. A single GetMetricData call can include as many as 500 MetricDataQuery structures.
  name: MetricDataQueries
  type: array
- description: The time stamp indicating the earliest data to be returned.
  name: StartTime
  type: string
- description: The time stamp indicating the latest data to be returned.
  name: EndTime
  type: string
- description: Include this value if it was returned by the previous GetMetricData operation.
  name: NextToken
  type: string
- description: The order in which data points should be returned.
  name: ScanBy
  type: string
- description: The maximum number of data points the request should return before paginating.
  name: MaxDatapoints
  type: integer
- description: ''
  name: LabelOptions
  type: object
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-get-metric-data-input-schema.json
slug: cloudwatch-get-metric-data-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetMetricDataInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricDataQueries\": {\n      \"type\": \"array\",\n      \"description\": \"The metric queries to be returned. A single GetMetricData call can include as many as 500 MetricDataQuery structures.\"\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time stamp indicating the earliest data to be returned.\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time stamp indicating the latest data to be returned.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Include this value if it was returned by the previous GetMetricData operation.\"\n    },\n    \"ScanBy\": {\n      \"type\": \"string\",\n      \"description\": \"The order in which data points should be returned.\"\n    },\n    \"MaxDatapoints\": {\n     \
  \ \"type\": \"integer\",\n      \"description\": \"The maximum number of data points the request should return before paginating.\"\n    },\n    \"LabelOptions\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-get-metric-data-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: GetMetricDataInput
---

---
description: Details about a metric. A metric is an aggregation of the values of a measure for a dimension value, such as <i>availability</i> in the <i>us-east-1</i> Region.
layout: schema
name: TimeSeries
properties_list:
- description: ''
  name: TimeSeriesId
  type: object
- description: ''
  name: DimensionList
  type: object
- description: ''
  name: MetricValueList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-time-series-schema.json
slug: amazon-lookout-for-metrics-time-series
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-time-series-schema.json\",\n  \"title\": \"TimeSeries\",\n  \"description\": \"Details about a metric. A metric is an aggregation of the values of a measure for a dimension value, such as <i>availability</i> in the <i>us-east-1</i> Region.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TimeSeriesId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSeriesId\"\n        },\n        {\n          \"description\": \"The ID of the metric.\"\n        }\n      ]\n    },\n    \"DimensionList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionNameValueList\"\n        },\n        {\n          \"description\": \"The dimensions of the metric.\"\n        }\n      ]\n    },\n    \"MetricValueList\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricValueList\"\n        },\n        {\n          \"description\": \"The values for the metric.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TimeSeriesId\",\n    \"DimensionList\",\n    \"MetricValueList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-time-series-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: TimeSeries
---

---
description: UpdateMetricSetRequest schema from Amazon Lookout for Metrics API
layout: schema
name: UpdateMetricSetRequest
properties_list:
- description: ''
  name: MetricSetArn
  type: object
- description: ''
  name: MetricSetDescription
  type: object
- description: ''
  name: MetricList
  type: object
- description: ''
  name: Offset
  type: object
- description: ''
  name: TimestampColumn
  type: object
- description: ''
  name: DimensionList
  type: object
- description: ''
  name: MetricSetFrequency
  type: object
- description: ''
  name: MetricSource
  type: object
- description: ''
  name: DimensionFilterList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-update-metric-set-request-schema.json
slug: amazon-lookout-for-metrics-update-metric-set-request
source_filename: amazon-lookout-for-metrics-update-metric-set-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-update-metric-set-request-schema.json\",\n  \"title\": \"UpdateMetricSetRequest\",\n  \"description\": \"UpdateMetricSetRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the dataset to update.\"\n        }\n      ]\n    },\n    \"MetricSetDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetDescription\"\n        },\n        {\n          \"description\": \"The dataset's description.\"\n        }\n      ]\n    },\n    \"MetricList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricList\"\
  \n        },\n        {\n          \"description\": \"The metric list.\"\n        }\n      ]\n    },\n    \"Offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Offset\"\n        },\n        {\n          \"description\": \"After an interval ends, the amount of seconds that the detector waits before importing data. Offset is only supported for S3, Redshift, Athena and datasources.\"\n        }\n      ]\n    },\n    \"TimestampColumn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampColumn\"\n        },\n        {\n          \"description\": \"The timestamp column.\"\n        }\n      ]\n    },\n    \"DimensionList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionList\"\n        },\n        {\n          \"description\": \"The dimension list.\"\n        }\n      ]\n    },\n    \"MetricSetFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Frequency\"\
  \n        },\n        {\n          \"description\": \"The dataset's interval.\"\n        }\n      ]\n    },\n    \"MetricSource\": {\n      \"$ref\": \"#/components/schemas/MetricSource\"\n    },\n    \"DimensionFilterList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetDimensionFilterList\"\n        },\n        {\n          \"description\": \"Describes a list of filters for choosing specific dimensions and specific values. Each filter consists of the dimension and one of its values that you want to include. When multiple dimensions or values are specified, the dimensions are joined with an AND operation and the values are joined with an OR operation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MetricSetArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-update-metric-set-request-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: UpdateMetricSetRequest
---

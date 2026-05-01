---
description: DescribeMetricSetResponse schema from Amazon Lookout for Metrics API
layout: schema
name: DescribeMetricSetResponse
properties_list:
- description: ''
  name: MetricSetArn
  type: object
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: MetricSetName
  type: object
- description: ''
  name: MetricSetDescription
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: LastModificationTime
  type: object
- description: ''
  name: Offset
  type: object
- description: ''
  name: MetricList
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
  name: Timezone
  type: object
- description: ''
  name: MetricSource
  type: object
- description: ''
  name: DimensionFilterList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-describe-metric-set-response-schema.json
slug: amazon-lookout-for-metrics-describe-metric-set-response
source_filename: amazon-lookout-for-metrics-describe-metric-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-describe-metric-set-response-schema.json\",\n  \"title\": \"DescribeMetricSetResponse\",\n  \"description\": \"DescribeMetricSetResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the dataset.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the detector that contains the dataset.\"\n        }\n      ]\n    },\n    \"MetricSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetName\"\
  \n        },\n        {\n          \"description\": \"The name of the dataset.\"\n        }\n      ]\n    },\n    \"MetricSetDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetDescription\"\n        },\n        {\n          \"description\": \"The dataset's description.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the dataset was created.\"\n        }\n      ]\n    },\n    \"LastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the dataset was last modified.\"\n        }\n      ]\n    },\n    \"Offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Offset\"\n        },\n        {\n          \"description\": \"After\
  \ an interval ends, the amount of seconds that the detector waits before importing data. Offset is only supported for S3, Redshift, Athena and datasources.\"\n        }\n      ]\n    },\n    \"MetricList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricList\"\n        },\n        {\n          \"description\": \"A list of the metrics defined by the dataset.\"\n        }\n      ]\n    },\n    \"TimestampColumn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampColumn\"\n        },\n        {\n          \"description\": \"Contains information about the column used for tracking time in your source data.\"\n        }\n      ]\n    },\n    \"DimensionList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionList\"\n        },\n        {\n          \"description\": \"A list of the dimensions chosen for analysis.\"\n        }\n      ]\n    },\n    \"MetricSetFrequency\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Frequency\"\n        },\n        {\n          \"description\": \"The interval at which the data will be analyzed for anomalies.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timezone\"\n        },\n        {\n          \"description\": \"The time zone in which the dataset's data was recorded.\"\n        }\n      ]\n    },\n    \"MetricSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSource\"\n        },\n        {\n          \"description\": \"Contains information about the dataset's source data.\"\n        }\n      ]\n    },\n    \"DimensionFilterList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetDimensionFilterList\"\n        },\n        {\n          \"description\": \"The dimensions and their values that were used to filter the dataset.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-describe-metric-set-response-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DescribeMetricSetResponse
---

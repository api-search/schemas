---
description: CreateMetricSetRequest schema from Amazon Lookout for Metrics API
layout: schema
name: CreateMetricSetRequest
properties_list:
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
  name: Timezone
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: DimensionFilterList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-create-metric-set-request-schema.json
slug: amazon-lookout-for-metrics-create-metric-set-request
source_filename: amazon-lookout-for-metrics-create-metric-set-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-create-metric-set-request-schema.json\",\n  \"title\": \"CreateMetricSetRequest\",\n  \"description\": \"CreateMetricSetRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the anomaly detector that will use the dataset.\"\n        }\n      ]\n    },\n    \"MetricSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetName\"\n        },\n        {\n          \"description\": \"The name of the dataset.\"\n        }\n      ]\n    },\n    \"MetricSetDescription\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/MetricSetDescription\"\n        },\n        {\n          \"description\": \"A description of the dataset you are creating.\"\n        }\n      ]\n    },\n    \"MetricList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricList\"\n        },\n        {\n          \"description\": \"A list of metrics that the dataset will contain.\"\n        }\n      ]\n    },\n    \"Offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Offset\"\n        },\n        {\n          \"description\": \"After an interval ends, the amount of seconds that the detector waits before importing data. Offset is only supported for S3, Redshift, Athena and datasources.\"\n        }\n      ]\n    },\n    \"TimestampColumn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampColumn\"\n        },\n        {\n          \"description\": \"Contains information about the column used for tracking\
  \ time in your source data.\"\n        }\n      ]\n    },\n    \"DimensionList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionList\"\n        },\n        {\n          \"description\": \"A list of the fields you want to treat as dimensions.\"\n        }\n      ]\n    },\n    \"MetricSetFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Frequency\"\n        },\n        {\n          \"description\": \"The frequency with which the source data will be analyzed for anomalies.\"\n        }\n      ]\n    },\n    \"MetricSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSource\"\n        },\n        {\n          \"description\": \"Contains information about how the source data should be interpreted.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timezone\"\n        },\n        {\n          \"description\"\
  : \"The time zone in which your source data was recorded.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of <a href=\\\"https://docs.aws.amazon.com/lookoutmetrics/latest/dev/detectors-tags.html\\\">tags</a> to apply to the dataset.\"\n        }\n      ]\n    },\n    \"DimensionFilterList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetDimensionFilterList\"\n        },\n        {\n          \"description\": \"A list of filters that specify which data is kept for anomaly detection.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AnomalyDetectorArn\",\n    \"MetricSetName\",\n    \"MetricList\",\n    \"MetricSource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-create-metric-set-request-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: CreateMetricSetRequest
---

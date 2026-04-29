---
description: Contains information about a dataset.
layout: schema
name: MetricSetSummary
properties_list:
- description: ''
  name: MetricSetArn
  type: object
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: MetricSetDescription
  type: object
- description: ''
  name: MetricSetName
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: LastModificationTime
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-metric-set-summary-schema.json
slug: amazon-lookout-for-metrics-metric-set-summary
source_filename: amazon-lookout-for-metrics-metric-set-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-set-summary-schema.json\",\n  \"title\": \"MetricSetSummary\",\n  \"description\": \"Contains information about a dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the dataset.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the detector to which the dataset belongs.\"\n        }\n      ]\n    },\n    \"MetricSetDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetDescription\"\n \
  \       },\n        {\n          \"description\": \"The description of the dataset.\"\n        }\n      ]\n    },\n    \"MetricSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricSetName\"\n        },\n        {\n          \"description\": \"The name of the dataset.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the dataset was created.\"\n        }\n      ]\n    },\n    \"LastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the dataset was last modified.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The dataset's <a\
  \ href=\\\"https://docs.aws.amazon.com/lookoutmetrics/latest/dev/detectors-tags.html\\\">tags</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-set-summary-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: MetricSetSummary
---

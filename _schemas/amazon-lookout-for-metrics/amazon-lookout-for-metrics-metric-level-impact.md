---
description: Details about a measure affected by an anomaly.
layout: schema
name: MetricLevelImpact
properties_list:
- description: ''
  name: MetricName
  type: object
- description: ''
  name: NumTimeSeries
  type: object
- description: ''
  name: ContributionMatrix
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-metric-level-impact-schema.json
slug: amazon-lookout-for-metrics-metric-level-impact
source_filename: amazon-lookout-for-metrics-metric-level-impact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-level-impact-schema.json\",\n  \"title\": \"MetricLevelImpact\",\n  \"description\": \"Details about a measure affected by an anomaly.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \"The name of the measure.\"\n        }\n      ]\n    },\n    \"NumTimeSeries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of anomalous metrics for the measure.\"\n        }\n      ]\n    },\n    \"ContributionMatrix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContributionMatrix\"\
  \n        },\n        {\n          \"description\": \"Details about the dimensions that contributed to the anomaly.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-level-impact-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: MetricLevelImpact
---

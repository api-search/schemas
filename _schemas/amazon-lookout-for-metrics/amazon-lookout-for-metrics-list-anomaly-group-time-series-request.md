---
description: ListAnomalyGroupTimeSeriesRequest schema from Amazon Lookout for Metrics API
layout: schema
name: ListAnomalyGroupTimeSeriesRequest
properties_list:
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: AnomalyGroupId
  type: object
- description: ''
  name: MetricName
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-list-anomaly-group-time-series-request-schema.json
slug: amazon-lookout-for-metrics-list-anomaly-group-time-series-request
source_filename: amazon-lookout-for-metrics-list-anomaly-group-time-series-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-anomaly-group-time-series-request-schema.json\",\n  \"title\": \"ListAnomalyGroupTimeSeriesRequest\",\n  \"description\": \"ListAnomalyGroupTimeSeriesRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the anomaly detector.\"\n        }\n      ]\n    },\n    \"AnomalyGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"The ID of the anomaly group.\"\n        }\n      ]\n    },\n    \"MetricName\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \"The name of the measure field.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Specify the pagination token that's returned by a previous request to retrieve the next page of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AnomalyDetectorArn\",\n    \"AnomalyGroupId\",\n    \"MetricName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-anomaly-group-time-series-request-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ListAnomalyGroupTimeSeriesRequest
---

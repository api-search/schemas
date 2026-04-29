---
description: ListAnomalyGroupTimeSeriesResponse schema from Amazon Lookout for Metrics API
layout: schema
name: ListAnomalyGroupTimeSeriesResponse
properties_list:
- description: ''
  name: AnomalyGroupId
  type: object
- description: ''
  name: MetricName
  type: object
- description: ''
  name: TimestampList
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: TimeSeriesList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-list-anomaly-group-time-series-response-schema.json
slug: amazon-lookout-for-metrics-list-anomaly-group-time-series-response
source_filename: amazon-lookout-for-metrics-list-anomaly-group-time-series-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-anomaly-group-time-series-response-schema.json\",\n  \"title\": \"ListAnomalyGroupTimeSeriesResponse\",\n  \"description\": \"ListAnomalyGroupTimeSeriesResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"The ID of the anomaly group.\"\n        }\n      ]\n    },\n    \"MetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \"The name of the measure field.\"\n        }\n      ]\n    },\n    \"TimestampList\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/TimestampList\"\n        },\n        {\n          \"description\": \"Timestamps for the anomalous metrics.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token that's included if more results are available.\"\n        }\n      ]\n    },\n    \"TimeSeriesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSeriesList\"\n        },\n        {\n          \"description\": \"A list of anomalous metrics.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-anomaly-group-time-series-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ListAnomalyGroupTimeSeriesResponse
---

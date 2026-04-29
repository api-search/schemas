---
description: ListAnomalyDetectorsResponse schema from Amazon Lookout for Metrics API
layout: schema
name: ListAnomalyDetectorsResponse
properties_list:
- description: ''
  name: AnomalyDetectorSummaryList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-list-anomaly-detectors-response-schema.json
slug: amazon-lookout-for-metrics-list-anomaly-detectors-response
source_filename: amazon-lookout-for-metrics-list-anomaly-detectors-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-anomaly-detectors-response-schema.json\",\n  \"title\": \"ListAnomalyDetectorsResponse\",\n  \"description\": \"ListAnomalyDetectorsResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorSummaryList\"\n        },\n        {\n          \"description\": \"A list of anomaly detectors in the account in the current region.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If the response is truncated, the service returns this token. To retrieve the next\
  \ set of results, use the token in the next request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-anomaly-detectors-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ListAnomalyDetectorsResponse
---

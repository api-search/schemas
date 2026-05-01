---
description: ListMetricSetsRequest schema from Amazon Lookout for Metrics API
layout: schema
name: ListMetricSetsRequest
properties_list:
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-list-metric-sets-request-schema.json
slug: amazon-lookout-for-metrics-list-metric-sets-request
source_filename: amazon-lookout-for-metrics-list-metric-sets-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-metric-sets-request-schema.json\",\n  \"title\": \"ListMetricSetsRequest\",\n  \"description\": \"ListMetricSetsRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the anomaly detector containing the metrics sets to list.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If the result of the previous request was truncated, the response includes a <code>NextToken</code>. To retrieve the next set of results, use the token in the next request. Tokens expire after 24 hours.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-metric-sets-request-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ListMetricSetsRequest
---

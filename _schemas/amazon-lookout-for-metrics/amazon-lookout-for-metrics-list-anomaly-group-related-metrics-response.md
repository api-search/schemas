---
description: ListAnomalyGroupRelatedMetricsResponse schema from Amazon Lookout for Metrics API
layout: schema
name: ListAnomalyGroupRelatedMetricsResponse
properties_list:
- description: ''
  name: InterMetricImpactList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-list-anomaly-group-related-metrics-response-schema.json
slug: amazon-lookout-for-metrics-list-anomaly-group-related-metrics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-anomaly-group-related-metrics-response-schema.json\",\n  \"title\": \"ListAnomalyGroupRelatedMetricsResponse\",\n  \"description\": \"ListAnomalyGroupRelatedMetricsResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InterMetricImpactList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterMetricImpactList\"\n        },\n        {\n          \"description\": \"Aggregated details about the measures contributing to the anomaly group, and the measures potentially impacted by the anomaly group.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\"\
  : \"The pagination token that's included if more results are available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-anomaly-group-related-metrics-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ListAnomalyGroupRelatedMetricsResponse
---

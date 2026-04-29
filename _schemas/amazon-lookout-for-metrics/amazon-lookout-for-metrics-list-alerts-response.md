---
description: ListAlertsResponse schema from Amazon Lookout for Metrics API
layout: schema
name: ListAlertsResponse
properties_list:
- description: ''
  name: AlertSummaryList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-list-alerts-response-schema.json
slug: amazon-lookout-for-metrics-list-alerts-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-alerts-response-schema.json\",\n  \"title\": \"ListAlertsResponse\",\n  \"description\": \"ListAlertsResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlertSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertSummaryList\"\n        },\n        {\n          \"description\": \"Contains information about an alert.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If the response is truncated, the service returns this token. To retrieve the next set of results, use this token in the next request.\"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-list-alerts-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ListAlertsResponse
---

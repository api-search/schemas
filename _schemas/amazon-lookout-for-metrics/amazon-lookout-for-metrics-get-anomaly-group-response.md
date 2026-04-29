---
description: GetAnomalyGroupResponse schema from Amazon Lookout for Metrics API
layout: schema
name: GetAnomalyGroupResponse
properties_list:
- description: ''
  name: AnomalyGroup
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-get-anomaly-group-response-schema.json
slug: amazon-lookout-for-metrics-get-anomaly-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-anomaly-group-response-schema.json\",\n  \"title\": \"GetAnomalyGroupResponse\",\n  \"description\": \"GetAnomalyGroupResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyGroup\"\n        },\n        {\n          \"description\": \"Details about the anomaly group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-anomaly-group-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: GetAnomalyGroupResponse
---

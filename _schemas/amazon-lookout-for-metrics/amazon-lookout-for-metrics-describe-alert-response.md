---
description: DescribeAlertResponse schema from Amazon Lookout for Metrics API
layout: schema
name: DescribeAlertResponse
properties_list:
- description: ''
  name: Alert
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-describe-alert-response-schema.json
slug: amazon-lookout-for-metrics-describe-alert-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-describe-alert-response-schema.json\",\n  \"title\": \"DescribeAlertResponse\",\n  \"description\": \"DescribeAlertResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alert\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alert\"\n        },\n        {\n          \"description\": \"Contains information about an alert.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-describe-alert-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DescribeAlertResponse
---

---
description: MetricNameList schema from Amazon Lookout for Metrics API
layout: schema
name: MetricNameList
properties_list: []
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-metric-name-list-schema.json
slug: amazon-lookout-for-metrics-metric-name-list
source_filename: amazon-lookout-for-metrics-metric-name-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-name-list-schema.json\",\n  \"title\": \"MetricNameList\",\n  \"description\": \"MetricNameList schema from Amazon Lookout for Metrics API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/MetricName\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 5\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-name-list-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: MetricNameList
---

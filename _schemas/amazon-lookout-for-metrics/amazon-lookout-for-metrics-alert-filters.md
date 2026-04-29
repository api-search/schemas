---
description: The configuration of the alert filters.
layout: schema
name: AlertFilters
properties_list:
- description: ''
  name: MetricList
  type: object
- description: ''
  name: DimensionFilterList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-alert-filters-schema.json
slug: amazon-lookout-for-metrics-alert-filters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-alert-filters-schema.json\",\n  \"title\": \"AlertFilters\",\n  \"description\": \"The configuration of the alert filters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricNameList\"\n        },\n        {\n          \"description\": \"The list of measures that you want to get alerts for.\"\n        }\n      ]\n    },\n    \"DimensionFilterList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionFilterList\"\n        },\n        {\n          \"description\": \"The list of DimensionFilter objects that are used for dimension-based filtering.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-alert-filters-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AlertFilters
---

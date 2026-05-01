---
description: Describes a list of filters for choosing a subset of dimension values. Each filter consists of the dimension and one of its values that you want to include. When multiple dimensions or values are specified, the dimensions are joined with an AND operation and the values are joined with an OR operation.
layout: schema
name: MetricSetDimensionFilter
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: FilterList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-metric-set-dimension-filter-schema.json
slug: amazon-lookout-for-metrics-metric-set-dimension-filter
source_filename: amazon-lookout-for-metrics-metric-set-dimension-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-set-dimension-filter-schema.json\",\n  \"title\": \"MetricSetDimensionFilter\",\n  \"description\": \"Describes a list of filters for choosing a subset of dimension values. Each filter consists of the dimension and one of its values that you want to include. When multiple dimensions or values are specified, the dimensions are joined with an AND operation and the values are joined with an OR operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"The dimension that you want to filter on.\"\n        }\n      ]\n    },\n    \"FilterList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\
  \n        },\n        {\n          \"description\": \"The list of filters that you are applying.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-metric-set-dimension-filter-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: MetricSetDimensionFilter
---

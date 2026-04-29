---
description: Describes a filter for choosing a subset of dimension values. Each filter consists of the dimension that you want to include and the condition statement. The condition statement is specified in the <code>FilterOperation</code> object.
layout: schema
name: Filter
properties_list:
- description: ''
  name: DimensionValue
  type: object
- description: ''
  name: FilterOperation
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-filter-schema.json
slug: amazon-lookout-for-metrics-filter
source_filename: amazon-lookout-for-metrics-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"Describes a filter for choosing a subset of dimension values. Each filter consists of the dimension that you want to include and the condition statement. The condition statement is specified in the <code>FilterOperation</code> object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DimensionValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionValue\"\n        },\n        {\n          \"description\": \"The value that you want to include in the filter.\"\n        }\n      ]\n    },\n    \"FilterOperation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterOperation\"\n        },\n        {\n          \"description\"\
  : \"The condition to apply.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-filter-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: Filter
---

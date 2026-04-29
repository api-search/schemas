---
description: A dimension name and value.
layout: schema
name: DimensionNameValue
properties_list:
- description: ''
  name: DimensionName
  type: object
- description: ''
  name: DimensionValue
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-dimension-name-value-schema.json
slug: amazon-lookout-for-metrics-dimension-name-value
source_filename: amazon-lookout-for-metrics-dimension-name-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-name-value-schema.json\",\n  \"title\": \"DimensionNameValue\",\n  \"description\": \"A dimension name and value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DimensionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"The name of the dimension.\"\n        }\n      ]\n    },\n    \"DimensionValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionValue\"\n        },\n        {\n          \"description\": \"The value of the dimension.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DimensionName\",\n    \"DimensionValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-name-value-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DimensionNameValue
---

---
description: The dimension filter, containing DimensionName and DimensionValueList.
layout: schema
name: DimensionFilter
properties_list:
- description: ''
  name: DimensionName
  type: object
- description: ''
  name: DimensionValueList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-dimension-filter-schema.json
slug: amazon-lookout-for-metrics-dimension-filter
source_filename: amazon-lookout-for-metrics-dimension-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-filter-schema.json\",\n  \"title\": \"DimensionFilter\",\n  \"description\": \"The dimension filter, containing DimensionName and DimensionValueList.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DimensionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"The name of the dimension to filter on.\"\n        }\n      ]\n    },\n    \"DimensionValueList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionValueList\"\n        },\n        {\n          \"description\": \"The list of values for the dimension specified in DimensionName that you want to filter on.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-filter-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DimensionFilter
---

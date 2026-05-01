---
description: Details about a dimension that contributed to an anomaly.
layout: schema
name: DimensionContribution
properties_list:
- description: ''
  name: DimensionName
  type: object
- description: ''
  name: DimensionValueContributionList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-dimension-contribution-schema.json
slug: amazon-lookout-for-metrics-dimension-contribution
source_filename: amazon-lookout-for-metrics-dimension-contribution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-contribution-schema.json\",\n  \"title\": \"DimensionContribution\",\n  \"description\": \"Details about a dimension that contributed to an anomaly.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DimensionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnName\"\n        },\n        {\n          \"description\": \"The name of the dimension.\"\n        }\n      ]\n    },\n    \"DimensionValueContributionList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionValueContributionList\"\n        },\n        {\n          \"description\": \"A list of dimension values that contributed to the anomaly.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-contribution-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DimensionContribution
---

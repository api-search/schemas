---
description: The severity of a value of a dimension that contributed to an anomaly.
layout: schema
name: DimensionValueContribution
properties_list:
- description: ''
  name: DimensionValue
  type: object
- description: ''
  name: ContributionScore
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-dimension-value-contribution-schema.json
slug: amazon-lookout-for-metrics-dimension-value-contribution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-value-contribution-schema.json\",\n  \"title\": \"DimensionValueContribution\",\n  \"description\": \"The severity of a value of a dimension that contributed to an anomaly.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DimensionValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionValue\"\n        },\n        {\n          \"description\": \"The value of the dimension.\"\n        }\n      ]\n    },\n    \"ContributionScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Score\"\n        },\n        {\n          \"description\": \"The severity score of the value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-value-contribution-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DimensionValueContribution
---

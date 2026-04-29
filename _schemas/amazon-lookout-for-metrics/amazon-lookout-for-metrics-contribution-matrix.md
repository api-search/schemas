---
description: Details about dimensions that contributed to an anomaly.
layout: schema
name: ContributionMatrix
properties_list:
- description: ''
  name: DimensionContributionList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-contribution-matrix-schema.json
slug: amazon-lookout-for-metrics-contribution-matrix
source_filename: amazon-lookout-for-metrics-contribution-matrix-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-contribution-matrix-schema.json\",\n  \"title\": \"ContributionMatrix\",\n  \"description\": \"Details about dimensions that contributed to an anomaly.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DimensionContributionList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionContributionList\"\n        },\n        {\n          \"description\": \"A list of contributing dimensions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-contribution-matrix-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: ContributionMatrix
---

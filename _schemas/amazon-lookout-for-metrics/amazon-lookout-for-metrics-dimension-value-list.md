---
description: DimensionValueList schema from Amazon Lookout for Metrics API
layout: schema
name: DimensionValueList
properties_list: []
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-dimension-value-list-schema.json
slug: amazon-lookout-for-metrics-dimension-value-list
source_filename: amazon-lookout-for-metrics-dimension-value-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-value-list-schema.json\",\n  \"title\": \"DimensionValueList\",\n  \"description\": \"DimensionValueList schema from Amazon Lookout for Metrics API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/DimensionValue\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 10\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-dimension-value-list-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DimensionValueList
---

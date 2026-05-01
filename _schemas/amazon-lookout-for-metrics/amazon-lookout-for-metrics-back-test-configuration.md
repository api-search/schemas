---
description: Settings for backtest mode.
layout: schema
name: BackTestConfiguration
properties_list:
- description: ''
  name: RunBackTestMode
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-back-test-configuration-schema.json
slug: amazon-lookout-for-metrics-back-test-configuration
source_filename: amazon-lookout-for-metrics-back-test-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-back-test-configuration-schema.json\",\n  \"title\": \"BackTestConfiguration\",\n  \"description\": \"Settings for backtest mode.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RunBackTestMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Run a backtest instead of monitoring new data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RunBackTestMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-back-test-configuration-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: BackTestConfiguration
---

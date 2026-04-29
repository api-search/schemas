---
description: The metric you want to retain. Dimensions are optional.
layout: schema
name: MetricToRetain
properties_list:
- description: ''
  name: metric
  type: object
- description: ''
  name: metricDimension
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-metric-to-retain-schema.json
slug: iot-device-defender-metric-to-retain
source_filename: iot-device-defender-metric-to-retain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-metric-to-retain-schema.json\",\n  \"title\": \"MetricToRetain\",\n  \"description\": \"The metric you want to retain. Dimensions are optional.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BehaviorMetric\"\n        },\n        {\n          \"description\": \"What is measured by the behavior.\"\n        }\n      ]\n    },\n    \"metricDimension\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricDimension\"\n        },\n        {\n          \"description\": \"The dimension of a metric. This can't be used with custom metrics.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"metric\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-metric-to-retain-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: MetricToRetain
---

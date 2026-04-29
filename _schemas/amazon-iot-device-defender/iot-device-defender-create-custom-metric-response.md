---
description: CreateCustomMetricResponse schema
layout: schema
name: CreateCustomMetricResponse
properties_list:
- description: ''
  name: metricName
  type: object
- description: ''
  name: metricArn
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-custom-metric-response-schema.json
slug: iot-device-defender-create-custom-metric-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-custom-metric-response-schema.json\",\n  \"title\": \"CreateCustomMetricResponse\",\n  \"description\": \"CreateCustomMetricResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \" The name of the custom metric to be used in the metric report. \"\n        }\n      ]\n    },\n    \"metricArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomMetricArn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Number (ARN) of the custom metric. For example, <code>arn:<i>aws-partition</i>:iot:<i>region</i>:<i>accountId</i>:custommetric/<i>metricName</i>\
  \ </code> \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-custom-metric-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateCustomMetricResponse
---

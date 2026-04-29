---
description: DescribeCustomMetricResponse schema
layout: schema
name: DescribeCustomMetricResponse
properties_list:
- description: ''
  name: metricName
  type: object
- description: ''
  name: metricArn
  type: object
- description: ''
  name: metricType
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-custom-metric-response-schema.json
slug: iot-device-defender-describe-custom-metric-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-custom-metric-response-schema.json\",\n  \"title\": \"DescribeCustomMetricResponse\",\n  \"description\": \"DescribeCustomMetricResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \" The name of the custom metric. \"\n        }\n      ]\n    },\n    \"metricArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomMetricArn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Number (ARN) of the custom metric. \"\n        }\n      ]\n    },\n    \"metricType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomMetricType\"\
  \n        },\n        {\n          \"description\": \"<p> The type of the custom metric. </p> <important> <p>The type <code>number</code> only takes a single metric value as an input, but while submitting the metrics value in the DeviceMetrics report, it must be passed as an array with a single value.</p> </important>\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomMetricDisplayName\"\n        },\n        {\n          \"description\": \" Field represents a friendly name in the console for the custom metric; doesn't have to be unique. Don't use this name as the metric identifier in the device metric report. Can be updated. \"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The creation date of the custom metric in milliseconds since epoch. \"\n        }\n  \
  \    ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The time the custom metric was last modified in milliseconds since epoch. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-custom-metric-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeCustomMetricResponse
---
